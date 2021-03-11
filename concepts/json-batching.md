---
title: Combinar várias solicitações em uma chamada HTTP usando processamento JSON em lotes
description: 'Os lotes JSON permitem otimizar seu aplicativo combinando várias solicitações em um único objeto JSON. Por exemplo, um cliente talvez queira criar um modo de exibição de dados não relacionados, como:'
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 4e1ad5734d0fefe2cdb7634e461ee9f297aae93e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721569"
---
# <a name="combine-multiple-requests-in-one-http-call-using-json-batching"></a>Combinar várias solicitações em uma chamada HTTP usando processamento JSON em lotes

Os lotes JSON permitem otimizar seu aplicativo combinando várias solicitações em um único objeto JSON. Por exemplo, um cliente talvez queira criar um modo de exibição de dados não relacionados, como:

1. Uma imagem armazenada no OneDrive
2. Uma lista de tarefas de Planejador
3. O calendário de um grupo

Combinar essas três solicitações individuais em uma única solicitação em lote pode economizar latência da rede significativa para o aplicativo.

> [!VIDEO https://www.youtube-nocookie.com/embed/tzWGOp8zYh8]

## <a name="first-json-batch-request"></a>Primeira solicitação JSON em lotes

Primeiro você cria a solicitação JSON em lote do exemplo anterior. Nesse cenário, as solicitações individuais não são interdependentes de qualquer forma e, portanto, podem ser colocadas na solicitação em lotes em qualquer ordem.

```http
POST https://graph.microsoft.com/v1.0/$batch
Accept: application/json
Content-Type: application/json
```

```json
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
    }
  ]
}
```

As respostas para solicitações em lote podem aparecer em uma ordem diferente. A propriedade `id` pode ser usada para correlacionar solicitações e respostas individuais.

```http
200 OK
Content-Type: application/json
```

```json
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

Solicitações de lote são sempre enviadas usando `POST` para o ponto de extremidade `/$batch`.

O corpo da solicitação JSON em lote consiste em um único objeto JSON com uma propriedade obrigatória: `requests`. A propriedade `requests` é uma matriz de solicitações individuais. Para cada solicitação individual, as propriedades `id`, `method` e `url` propriedades são necessárias.

A propriedade `id` funciona principalmente como um valor de correlação para associar solicitações a respostas individuais. Isso permite que o servidor processe solicitações em lote na ordem mais eficiente.

As propriedades `method` e `url` são exatamente o que você vê no início de qualquer solicitação HTTP. O método é o método HTTP e a URL é a URL de recurso para a qual a solicitação individual normalmente seria enviada.

As solicitações individuais podem, como opção, também conter uma propriedade `headers` e uma propriedade`body`. Essas duas propriedades geralmente são objetos JSON, conforme mostrado no exemplo anterior. Em alguns casos, o `body` pode ser um valor codificado como URL base64 em vez de um objeto JSON; por exemplo, quando o corpo é uma imagem. Quando um `body` está incluído na solicitação, o objeto `headers` deve conter um valor para `Content-Type`.

## <a name="response-format"></a>Formato de resposta

O formato de resposta para solicitações de lote JSON é semelhante ao formato da solicitação. A seguir estão as principais diferenças:

* A propriedade no objeto JSON principal é denominada `responses` em vez de `requests`.
* As respostas individuais podem aparecer em uma ordem diferente das solicitações.
* Em vez de `method` e `url`, as respostas individuais têm uma propriedade `status`. O valor de `status` é um número que representa o código de status HTTP.

O código de status em uma resposta de lote geralmente é `200` ou `400`. Se a solicitação em lotes em si for mal formada, o código de status será `400`. Se a solicitação de lote for analisável, o código de status será `200`. Um código de status `200` na resposta em lote não indica que as solicitações individuais no lote são bem-sucedidas. É por isso que cada resposta individual na propriedade `responses` tem um código de status.

## <a name="sequencing-requests-with-the-dependson-property"></a>Solicitações de sequenciamento com a propriedade dependsOn

As solicitações individuais podem ser executadas em uma ordem especificada pela propriedade `dependsOn`. Essa propriedade é uma matriz de cadeias de caracteres que fazem referência a `id` de uma solicitação individual diferente. Por esse motivo, os valores de `id` precisam ser exclusivos. Por exemplo, na solicitação a seguir, o cliente está especificando que as solicitações 1 e 3 devem ser executadas primeiro, em seguida a solicitação 2 e a solicitação 4.

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
      "id": "3",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "4",
      "dependsOn": [ "2" ],
      "method": "GET",
      "url": "..."
    }
  ]
}
```

Se uma solicitação individual falhar, qualquer solicitação que dependa dessa solicitação falhará com código de status `424` (dependência com falha).

## <a name="bypassing-url-length-limitations-with-batching"></a>Ignorar limitações de tamanho de URL com processamento em lotes

Um caso de uso adicional para processamento em lotes JSON é ignorar as limitações de tamanho de URL. Em casos nos quais a cláusula de filtro é complexa, o comprimento de URL pode superar limitações incorporadas a navegadores ou a outros clientes HTTP. Você pode usar processamento em lotes JSON como solução alternativa para executar essas solicitações já que a URL longa simplesmente torna-se parte da carga da solicitação.

## <a name="known-issues"></a>Problemas conhecidos

Para obter uma lista de limitações atuais relacionadas a lotes, veja [problemas conhecidos][batching-known-issues].

[batching-known-issues]: known-issues.md#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a>Confira também

Para mais informações a respeito do formato solicitação/resposta em lotes do JSON, leia [especificações da versão 4.01 do OData JSON Format](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#sec_BatchRequestsandResponses), seção _Solicitações e Respostas em Lote_.
