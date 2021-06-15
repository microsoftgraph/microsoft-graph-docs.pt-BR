---
author: JeremyKelley
ms.date: 09/10/2017
title: Sincronizar o conteúdo de uma unidade
localization_priority: Priority
ms.prod: sharepoint
description: Esse método permite que o seu aplicativo controle alterações em uma unidade e seus filhos com o passar do tempo.
doc_type: apiPageType
ms.openlocfilehash: bcf638e5217768012a7e361ebed3cd760ac079c0
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911309"
---
# <a name="track-changes-for-a-drive"></a>Controlar alterações para uma unidade

Namespace: microsoft.graph

Esse método permite que o seu aplicativo controle alterações em uma unidade e seus filhos com o passar do tempo.

Seu aplicativo começa chamando `delta` sem parâmetros. O serviço começa a enumerar a hierarquia da unidade, retornando páginas de itens e um `@odata.nextLink` ou `@odata.deltaLink`, conforme descrito abaixo. Seu aplicativo deve continuar chamando com o `@odata.nextLink` até que você não veja mais um `@odata.nextLink` retornado ou até que você veja uma resposta com um conjunto vazio de alterações.

Quando terminar de receber todas as alterações, você pode aplicá-las ao seu estado local. Para verificar se há alterações no futuro, chame `delta` novamente com o `@odata.deltaLink` da resposta anterior.

Itens excluídos são retornados com a [faceta `deleted`](../resources/deleted.md). Itens com esse conjunto de propriedades devem ser removidos do seu estado local. 

>**Observação:** você apenas deverá excluir uma pasta localmente se ela ficar vazia após a sincronização de todas as alterações.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Aplicativo | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a>Parâmetros de função

| Parâmetro   | Tipo  | Descrição                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| token  | string | Opcional. Quando não é especificado, enumera o estado da hierarquia atual. Quando é `latest`, retorna uma resposta vazia com o token delta mais recente. Quando é um token delta anterior, retorna o novo estado após o token.

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$select`, `$expand` e `$top` para personalizar as resposta.

## <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Driveitem](../resources/driveitem.md) no corpo da resposta.

Além da coleção de DriveItems, a resposta também incluirá uma das seguintes propriedades:

| Nome                 | Valor  | Descrição                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| **\@odata.nextLink**  | url    | Uma URL para recuperar a próxima página disponível de alterações, se houver alterações adicionais no conjunto atual.                                        |
| **\@odata.deltaLink** | url    | Um URL retornado em no lugar de **\@odata.nextLink** após todas as alterações atuais terem sido retornadas. Usado para ler o próximo conjunto de alterações no futuro.  |

## <a name="example-initial-request"></a>Exemplo (solicitação inicial)

Veja a seguir um exemplo de como chamar essa API para estabelecer seu estado local.

### <a name="request"></a>Solicitação

Veja a seguir um exemplo da solicitação inicial.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_first", "tags": "service.graph" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-first-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-first-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-first-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-first-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true, "scope": "file.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        },
        {
            "id": "2353010204ddgg",
            "name": "file5.txt",
            "deleted": { }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/delta(token=1230919asd190410jlka)"
}
```

Essa resposta inclui a primeira página de alterações e a propriedade **\@odata.nextLink** indica que há mais itens disponíveis no conjunto atual de itens. Seu aplicativo deve continuar a solicitar o valor de URL de **\@odata.nextLink** até que todas as páginas de itens tenham sido recuperadas.

## <a name="example-last-page-in-a-set"></a>Exemplo (última página de um conjunto)

Veja a seguir um exemplo de como chamar essa API para atualizar seu estado local.

### <a name="request"></a>Solicitação

Veja a seguir um exemplo da solicitação após a solicitação inicial.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-item-delta-last", "tags": "service.graph" }-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-last-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-last-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-last-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-last-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)", "scope": "file.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { },
            "deleted": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?(token='1230919asd190410jlka')"
}
```

Essa resposta indica que o item denominado `folder2` foi excluído e que o item `file.txt` foi adicionado ou modificado entre a solicitação inicial e essa solicitação para atualizar o estado local.

A página final dos itens incluirá a propriedade **\@odata.deltaLink**, que fornece a URL que pode ser usada posteriormente para recuperar alterações desde o conjunto atual de itens.

Pode haver casos em que o serviço não pode fornecer uma lista de alterações para um determinado token (por exemplo, se um cliente tentar reutilizar um token antigo depois de ter permanecido desconectado por um longo período, ou se o estado do servidor tiver mudado e um novo token for obrigatório). Nesses casos, o serviço retornará um erro `HTTP 410 Gone` com uma resposta de erro contendo um dos códigos de erro abaixo e um cabeçalho `Location` contendo um novo nextLink que inicia uma enumeração delta do zero. Depois de concluir a enumeração completa, compare os itens retornados com seu estado local e siga estas instruções.

| Tipo de erro                       | Instruções                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | Substitua todos os itens locais pela versão do servidor (incluindo exclusões) se você tiver certeza de que o serviço estava atualizado com suas alterações locais quando você sincronizou pela última vez. Carregue alterações locais que o servidor não conhece. |
| `resyncChangesUploadDifferences` | Carregue os itens locais que o serviço não retornou e carregue os arquivos que diferem da versão do servidor (mantendo ambas as cópias se você não tiver certeza de qual é a mais atual).                                       |

## <a name="retrieving-the-current-deltalink"></a>Recuperar o deltaLink atual

Em alguns cenários, pode ser útil solicitar o valor do deltaLink atual sem primeiro enumerar todos os itens que já estão na unidade.

Isso poderá ser útil se o seu aplicativo quiser apenas saber sobre as alterações e não quiser saber sobre os itens existentes. Para recuperar o deltaLink mais recente, chame `delta` com um parâmetro de cadeia de caracteres de consulta `?token=latest`.

**Observação: Se você estiver tentando manter uma representação local completa dos itens em uma pasta ou unidade, use `delta` para a enumeração inicial. Outros métodos, como fazer a paginação por meio da coleção `children` de uma pasta, não garantirá o retorno de todos os itens se ocorrerem gravações durante a enumeração. O uso de `delta` é a única maneira de garantir a leitura de todos os dados necessários.**

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-latest", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```msgraph-interactive
GET /me/drive/root/delta?token=latest
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-latest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-latest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-latest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-latest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- { "blockType": "response", "isEmpty": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a>Comentários

* O feed delta mostra o estado mais recente de cada item, e não cada alteração. Se um item tiver sido renomeado duas vezes, ele só aparecerá uma vez, com seu nome mais recente.
* O mesmo item pode aparecer mais de uma vez em um feed delta, por vários motivos. Você deve usar a última ocorrência que visualizar.
* A propriedade `parentReference` em itens não incluirá um valor para **path**. Isso ocorre porque a renomeação de uma pasta não faz com que os descendentes dessa pasta sejam retornados de **delta**. **Ao usar delta, você sempre deve controlar itens por id**.
* A consulta delta não retornará algumas propriedades DriveItem, dependendo da operação e do tipo de serviço, conforme mostrado nas tabelas a seguir.

    **OneDrive for Business**
    
    | Tipo de operação | Propriedades omitidas pela consulta delta |
    |---------|----------|
    | Criar/Modificar | `ctag`, `lastModifiedBy` |
    | Excluir | `ctag`, `lastModifiedBy`, `name` |


    **OneDrive (consumidor)**
    
    | Tipo de operação | Propriedades omitidas pela consulta delta |
    |---------|----------|
    | Criar/Modificar | n/d |
    | Excluir | `ctag`, `size` |

## <a name="scanning-permissions-hierarchies"></a>Hierarquias de permissões de verificação
Por padrão, a resposta da consulta delta incluirá o compartilhamento de informações de todos os itens da consulta que foram alterados, mesmo que herdem suas permissões dos pais e não tenham elas próprias alterações diretas de compartilhamento. Isso normalmente resulta em uma chamada de acompanhamento para obter os detalhes da permissão de cada item, e não apenas daqueles cujas informações de compartilhamento foram alteradas. Você pode otimizar sua compreensão de como as alterações de permissão acontecem adicionando o cabeçalho `Prefer: hierarchicalsharing` à sua solicitação de consulta delta.

Quando o cabeçalho `Prefer: hierarchicalsharing` é fornecido, as informações de compartilhamento serão retornadas para a raiz da hierarquia de permissões, bem como itens que possuam, explicitamente, alterações de compartilhamento. Nos casos onde a mudança de compartilhamento é remover o compartilhamento de um item, você encontrará uma faceta de compartilhamento vazia para diferenciar entre os itens que herdam de seus pais e aqueles que são únicos, mas sem links de compartilhamento. Você também verá essa faceta de compartilhamento vazia na raiz de uma hierarquia de permissões que não é compartilhada para estabelecer o escopo inicial.

Em muitos cenários de verificação, você pode estar interessado, especificamente, em alterações nas permissões. Para deixar claro na resposta da consulta delta quais alterações são resultados de alterações nas permissões, você pode fornecer o cabeçalho `Prefer: deltashowsharingchanges`. Quando esse cabeçalho é fornecido, todos os itens que aparecem na resposta da consulta delta devido a alterações de permissão, terão a anotação OData `@microsoft.graph.sharedChanged":"True"`. Esse recurso é aplicável ao SharePoint e ao OneDrive for Business, mas não às contas de consumidor do OneDrive.

> **Nota:** O uso do cabeçalho `Prefer: deltashowsharingchanges` requer que você use `Prefer: deltashowremovedasdeleted` e `Prefer: deltatraversepermissiongaps`. Esses valores de cabeçalho podem ser agrupados em um único cabeçalho: `Prefer: deltashowremovedasdeleted, deltatraversepermissiongaps, deltashowsharingchanges`.

## <a name="error-responses"></a>Respostas de erros

Além dos erros de ressincronização detalhados acima, confira os detalhes sobre como os erros são retornados em [Respostas de Erros][error-response].

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": [
  ]
} -->

