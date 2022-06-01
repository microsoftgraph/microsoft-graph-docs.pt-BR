---
title: Combinar várias solicitações em uma chamada HTTP usando processamento JSON em lotes
description: 'Os lotes JSON permitem otimizar seu aplicativo combinando várias solicitações em um único objeto JSON. Por exemplo, um cliente talvez queira criar um modo de exibição de dados não relacionados, como:'
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 52c50796722faf51c91b65d65a21b3b495566924
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819696"
---
# <a name="combine-multiple-requests-in-one-http-call-using-json-batching"></a>Combinar várias solicitações em uma chamada HTTP usando processamento JSON em lotes

Os lotes JSON permitem otimizar seu aplicativo combinando várias solicitações (até 20) em um único objeto JSON. Por exemplo, um cliente talvez queira criar um modo de exibição de dados não relacionados, como:

1. Uma imagem armazenada no OneDrive
2. Uma lista de tarefas de Planejador
3. O calendário de um grupo

Combinar essas três solicitações individuais em uma única solicitação em lote pode economizar latência da rede significativa para o aplicativo.

> [!VIDEO https://www.youtube-nocookie.com/embed/tzWGOp8zYh8]

## <a name="first-json-batch-request"></a>Primeira solicitação JSON em lotes

Primeiro você cria a solicitação JSON em lote do exemplo anterior. Nesse cenário, as solicitações individuais não são interdependentes de qualquer forma e, portanto, podem ser colocadas na solicitação em lotes em qualquer ordem.

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/$batch
Accept: application/json
Content-Type: application/json

{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "/me/drive/root:/{file}:/content"
    },
    {
      "id": "2",
      "method": "GET",
      "url": "/me/planner/tasks"
    },
    {
      "id": "3",
      "method": "GET",
      "url": "/groups/{id}/events"
    },
    {
      "id": "4",
      "url": "/me",
      "method": "PATCH",
      "body": {
        "city" : "Redmond"
      },
      "headers": {
        "Content-Type": "application/json"
      }
    },
    {
      "id": "5",
      "url": "users?$select=id,displayName,userPrincipalName&$filter=city eq null&$count=true",
      "method": "GET",
      "headers": {
        "ConsistencyLevel": "eventual"
      }
    }
  ]
}
```

As respostas às solicitações em lote podem aparecer em uma ordem diferente. A propriedade **id** pode ser usada para correlacionar solicitações e respostas individuais.

```http
200 OK
Content-Type: application/json

{
  "responses": [
    {
      "id": "1",
      "status": 302,
      "headers": {
        "location": "https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi"
      }
    },
    {
      "id": "3",
      "status": 401,
      "body": {
        "error": {
          "code": "Forbidden",
          "message": "..."
        }
      }
    },
    {
      "id": "5",
      "status": 200,
      "headers": {
        "OData-Version": "4.0",
      },
      "body": {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(id,displayName,userPrincipalName)",
        "@odata.count": 12,
        "value": [
          {
            "id": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "displayName": "Adele Vance",
            "userPrincipalName": "AdeleV@Contoso.com"
          }
        ]
      }
    },
    {
      "id": "2",
      "status": 200,
      "body": {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.plannerTask)",
        "value": []
      }
    },
    {
      "id": "4",
      "status": 204,
      "body": null
    }
  ]
}
```

## <a name="request-format"></a>Formato da solicitação

As solicitações em lote são sempre enviadas usando um **POST** para o `/$batch` ponto de extremidade.

Um corpo de solicitação em lote JSON consiste em um único objeto JSON com uma propriedade obrigatória: **solicitações**. A propriedade **solicitações** é uma coleção de solicitações individuais. Para cada solicitação individual, as propriedades a seguir podem ser passadas.


| Propriedade | Descrição |
|----------|-------------|
| id       | Obrigatório. Um valor de correlação para associar respostas individuais a solicitações. Esse valor permite que o servidor processe solicitações no lote na ordem mais eficiente.    |
| method   | Obrigatório. O método HTTP.    |
| url      | Obrigatório. A URL de recurso relativa para a qual a solicitação individual normalmente seria enviada. Portanto, enquanto o URL absoluto é `https://graph.microsoft.com/v1.0/users`, este URL é `/users`. |
| cabeçalhos   | Opcional, mas obrigatório quando o **corpo** é especificado. Um objeto JSON com o par chave/valor para os cabeçalhos. Por exemplo, quando o cabeçalho **ConsistencyLevel** for obrigatorio, essa propriedade será representada como `"headers": {"ConsistencyLevel": "eventual"}`. Quando o **corpo** é fornecido, um cabeçalho **Content-Type** deve ser incluído.    |
| corpo   | Opcional. Pode ser um objeto JSON ou um valor codificado por URL base64, por exemplo, quando o corpo é uma imagem. Quando um **corpo** é incluído na solicitação, o objeto **cabeçalhos** deve conter um valor para **Content-Type**. |

## <a name="response-format"></a>Formato de resposta

O formato de resposta para solicitações de lote JSON é semelhante ao formato da solicitação. A seguir estão as principais diferenças:

* A propriedade no objeto principal do JSON é nomeada **respostas** em oposição a **solicitações**.
* As respostas individuais podem aparecer em uma ordem diferente das solicitações.
* Em vez de **método** e **url**, as respostas individuais têm uma propriedade **status**. O valor de **status** é um número que representa o código de status HTTP.
* A propriedade **cabeçalhos** em cada resposta individual representa os cabeçalhos devolvidos pelo servidor, por exemplo, cabeçalhos de **Cache-Control** e **Content-Type**.

O código de status em uma resposta em lote geralmente é `200` ou `400`. Se a própria solicitação de lote estiver malformada, o código de status será `400`. Se a solicitação em lote for analisável, o código de status será `200`. Um código de status `200` na resposta do lote não indica que as solicitações individuais dentro do lote foram bem-sucedidas. É por isso que cada resposta individual na propriedade **respostas** tem um código de status.

## <a name="sequencing-requests-with-the-dependson-property"></a>Solicitações de sequenciamento com a propriedade dependsOn

As solicitações individuais podem ser executadas em uma ordem especificada usando a propriedade **dependOn**. Essa propriedade é uma matriz de strings que faz referência ao **id** de uma solicitação individual diferente. Por esse motivo, os valores para **id** devem ser exclusivos. Por exemplo, na solicitação a seguir, o cliente está especificando que as solicitações devem ser executadas na solicitação de pedido 1, depois na solicitação 3, na solicitação 2 e na solicitação 4.

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "2",
      "dependsOn": [ "1" ],
      "method": "GET",
      "url": "..."
    },
    {
      "id": "4",
      "dependsOn": [ "2" ],
      "method": "GET",
      "url": "..."
    },
    {
      "id": "3",
      "dependsOn": [ "4" ],
      "method": "GET",
      "url": "..."
    }
  ]
}
```

Se uma solicitação individual falhar, qualquer solicitação que dependa dessa solicitação falhará com código de status `424` (dependência com falha).

> [!TIP]
> O lote deve ser totalmente sequencial ou totalmente paralelo.

## <a name="bypassing-url-length-limitations-with-batching"></a>Ignorar limitações de tamanho de URL com processamento em lotes

Um caso de uso adicional para processamento em lotes JSON é ignorar as limitações de tamanho de URL. Em casos nos quais a cláusula de filtro é complexa, o comprimento de URL pode superar limitações incorporadas a navegadores ou a outros clientes HTTP. Você pode usar processamento em lotes JSON como solução alternativa para executar essas solicitações já que a URL longa simplesmente torna-se parte da carga da solicitação.

## <a name="batch-size-limitations"></a>Limitações de tamanho do lote

As solicitações em lote JSON estão atualmente limitadas a 20 solicitações individuais, além das seguintes limitações:

* Dependendo das APIs que fazem parte da solicitação em lote, os serviços subjacentes impõem seus próprios limites de restrição que afetam os aplicativos que usam o Microsoft Graph para acessá-los.
* As solicitações em um lote são avaliadas individualmente em relação aos limites de controle e, se alguma solicitação exceder os limites, ela falhará com um status de `429`.
* Os lotes direcionados aos recursos do Outlook (como correio e calendário) podem conter apenas quatro solicitações direcionadas à mesma caixa de correio. Para obter detalhes, confira [Limites de serviço do Outlook][throttling-outlook].

Para obter mais informações, confira [Limitação e envio em lote][throttling-and-batching].

## <a name="known-issues"></a>Problemas conhecidos

Para obter uma lista de limitações atuais relacionadas a lotes, veja [problemas conhecidos][batching-known-issues].

[batching-known-issues]: known-issues.md#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx
[throttling-and-batching]: throttling.md#throttling-and-batching
[throttling-outlook]: throttling.md#outlook-service-limits

## <a name="see-also"></a>Confira também

Para mais informações a respeito do formato solicitação/resposta em lotes do JSON, leia [especificações da versão 4.01 do OData JSON Format](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#sec_BatchRequestsandResponses), seção _Solicitações e Respostas em Lote_.
