---
author: learafa
description: Obtenha itens de lista recém-criados, atualizados ou excluídos sem precisar executar uma leitura completa de toda a coleção de itens.
title: 'lisItem: delta'
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: def214ca5ba9d633ba9835d3678350fd9cf6e04a
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549628"
---
# <a name="listitem-delta"></a>listItem: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha itens de lista recém-criados, atualizados ou excluídos [sem precisar](../resources/listitem.md) executar uma leitura completa de toda a coleção de itens.

Seu aplicativo começa chamando `delta` sem parâmetros.
O serviço começa a enumerar a hierarquia da lista, retornando páginas de itens e um **@odata.nextLink** ou um **@odata.deltaLink**.
Seu aplicativo deve continuar chamando com **o @odata.nextLink** até que você veja um **@odata.deltaLink** retornado.

Depois de receber todas as alterações, você poderá aplicá-las ao seu estado local.
Para verificar se há alterações no futuro, chame `delta` novamente com **o @odata.deltaLink** da resposta anterior.

O feed delta mostra o estado mais recente de cada item, e não cada alteração. Se um item tiver sido renomeado duas vezes, ele só será mostrado uma vez, com seu nome mais recente.
O mesmo item pode aparecer mais de uma vez em um feed delta, por vários motivos. Você deve usar a última ocorrência que visualizar.

Os itens excluídos são retornados com [a faceta excluída](../resources/deleted.md). Excluído indica que o item foi excluído e não pode ser restaurado.
Os itens com essa propriedade devem ser removidos do seu estado local.

> **Nota:** Você só deverá excluir uma pasta localmente se ela estiver vazia depois de sincronizar todas as alterações.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/lists/{listId}/items/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

Na URL da solicitação, você pode incluir o seguinte parâmetro de consulta opcional.

| Parâmetro    | Tipo   | Descrição                                                                                                                          |
|:-------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| token        | string | Opcional. Se não for especificado, enumerará o estado atual da hierarquia. If `latest`, retorna uma resposta vazia com o token delta mais recente. Se um token delta anterior, retornará um novo estado desde esse token.|

Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$select`, `$expand` e `$top` para personalizar as resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Cabeçalho       |Valor                    |
|-------------|-------------------------|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [listItem](../resources/listitem.md) no corpo da resposta.

Além de uma coleção de **objetos listItem** , a resposta também incluirá uma das propriedades a seguir.

| Nome                 | Valor  | Descrição                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| **@odata.nextLink**  | URL    | Uma URL para recuperar a próxima página disponível de alterações, se houver alterações adicionais no conjunto atual.                                        |
| **@odata.deltaLink** | URL    | Uma URL retornada no lugar de **@odata.nextLink** após o retorno de todas as alterações atuais. Usada para ler o próximo conjunto de alterações no futuro.  |

Em alguns casos, `410 Gone` `Location` `nextLink` o serviço retornará um código de resposta com uma resposta de erro que contém um dos códigos de erro a seguir e um cabeçalho contendo um novo que inicia uma nova enumeração delta. Isso ocorre quando o serviço não pode fornecer uma lista de alterações para um determinado token (por exemplo, se um cliente tentar reutilizar um token antigo depois de ser desconectado por um longo tempo ou se o estado do servidor tiver sido alterado e um novo token for necessário).

Depois que a enumeração completa for concluída, compare os itens retornados com o estado local e siga as instruções com base no tipo de erro.

| Tipo de erro                       | Instruções                                                                                                                               |
|:---------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | Substitua todos os itens locais por versões do servidor (incluindo exclusões) se tiver certeza de que o serviço estava atualizado com as alterações locais na última sincronização. Carregar alterações locais que o servidor não conhece. |
| `resyncChangesUploadDifferences` | Upload itens locais que o serviço não retornou e carregue itens que diferem das versões do servidor (mantenha ambas as cópias se você não tiver certeza de qual deles está mais atualizado).                                       |

Além dos erros de ressincronização e para obter mais detalhes sobre como os erros são retornados, consulte o Microsoft Graph tipos de recursos e respostas [de erro][error-response].

## <a name="examples"></a>Exemplos

### <a name="example-1-initial-request"></a>Exemplo 1: solicitação inicial

Veja a seguir um exemplo da solicitação inicial que mostra como chamar essa API para estabelecer seu estado local.

#### <a name="request"></a>Solicitação

A seguir está um exemplo da solicitação inicial.

<!-- { "blockType": "request", "name": "get_listItem_delta_first" } -->

```http
GET https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta
```

#### <a name="response"></a>Resposta

A seguir está um exemplo da resposta que inclui a primeira página de alterações e a propriedade **@odata.nextLink** que indica que não há mais itens disponíveis no conjunto atual de itens. Seu aplicativo deve continuar a solicitar o valor de URL de **@odata.nextLink** até que todas as páginas de itens tenham sido recuperadas.

<!-- { "blockType": "response", "name": "get_listItem_delta_first", "@odata.type": "microsoft.graph.listItem", "isCollection": true, "truncated": true, "scope": "site.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC066},756\"",
            "id": "1",
            "lastModifiedDateTime": "2021-10-14T23:27:27Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestFolder",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "1",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Folder"
            }
        },
        {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC067},756\"",
            "id": "2",
            "lastModifiedDateTime": "2021-10-14T23:27:27Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestItemA.txt",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "2",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Document"
            }
        },
        {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC068},756\"",
            "id": "3",
            "lastModifiedDateTime": "2021-10-14T23:27:27Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestItemB.txt",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "3",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Document"
            }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka"
}
```

### <a name="example-2-last-page-request"></a>Exemplo 2: solicitação da última página

Veja a seguir um exemplo de uma solicitação que mostra a última página em um conjunto e como chamar essa API para atualizar seu estado local.

#### <a name="request"></a>Solicitação

A seguir está um exemplo de uma solicitação após a solicitação inicial.

<!-- { "blockType": "request", "name": "get-listItem-delta-last" }-->

```http
GET https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka
```

#### <a name="response"></a>Resposta

A seguir está um exemplo da resposta que indica que o item nomeado foi excluído e o item `TestItemB.txt` `TestFolder` foi adicionado ou modificado entre a solicitação inicial e essa solicitação para atualizar o estado local.

A página final de itens incluirá a propriedade **@odata.deltaLink**, que fornece a URL que poderá ser usada posteriormente para recuperar alterações desde o conjunto atual de itens.


<!-- { "blockType": "response", "name": "get-listItem-delta-last", "truncated": true, "@odata.type": "microsoft.graph.listItem", "isCollection": true,  "scope": "site.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC066},756\"",
            "id": "1",
            "lastModifiedDateTime": "2016-03-21T20:01:37Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestFolder",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "1",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Folder"
            }
        },
        {
            "id": "3",
            "parentReference": {
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Document"
            },
            "deleted": {"state": "deleted"}
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka"
}
```

### <a name="example-3-delta-link-request"></a>Exemplo 3: solicitação de link delta

Em alguns cenários, pode ser `deltaLink` útil solicitar o valor atual sem primeiro enumerar todos os itens na lista. Isso pode ser útil se seu aplicativo só quiser saber sobre alterações e não precisar saber sobre itens existentes.
Para recuperar a chamada mais recente `deltaLink`, chame com `delta` o parâmetro de cadeia de caracteres de consulta `?token=latest`.

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "sites.read", "target": "action" } -->

```http
GET /sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=latest
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- { "blockType": "response", "name": "get-delta-latest", "isEmpty": true, "@odata.type": "microsoft.graph.listItem", "isCollection": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka"
}
```

## <a name="see-also"></a>Confira também
[Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview)

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath&quot;: &quot;ListItem/Get delta"
} -->
