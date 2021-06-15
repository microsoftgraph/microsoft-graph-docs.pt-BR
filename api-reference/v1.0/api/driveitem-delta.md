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
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="f92df-103">Controlar alterações para uma unidade</span><span class="sxs-lookup"><span data-stu-id="f92df-103">Track changes for a Drive</span></span>

<span data-ttu-id="f92df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f92df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f92df-105">Esse método permite que o seu aplicativo controle alterações em uma unidade e seus filhos com o passar do tempo.</span><span class="sxs-lookup"><span data-stu-id="f92df-105">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="f92df-p101">Seu aplicativo começa chamando `delta` sem parâmetros. O serviço começa a enumerar a hierarquia da unidade, retornando páginas de itens e um `@odata.nextLink` ou `@odata.deltaLink`, conforme descrito abaixo. Seu aplicativo deve continuar chamando com o `@odata.nextLink` até que você não veja mais um `@odata.nextLink` retornado ou até que você veja uma resposta com um conjunto vazio de alterações.</span><span class="sxs-lookup"><span data-stu-id="f92df-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="f92df-p102">Quando terminar de receber todas as alterações, você pode aplicá-las ao seu estado local. Para verificar se há alterações no futuro, chame `delta` novamente com o `@odata.deltaLink` da resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="f92df-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="f92df-p103">Itens excluídos são retornados com a [faceta `deleted`](../resources/deleted.md). Itens com esse conjunto de propriedades devem ser removidos do seu estado local.</span><span class="sxs-lookup"><span data-stu-id="f92df-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

><span data-ttu-id="f92df-113">**Observação:** você apenas deverá excluir uma pasta localmente se ela ficar vazia após a sincronização de todas as alterações.</span><span class="sxs-lookup"><span data-stu-id="f92df-113">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="f92df-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="f92df-114">Permissions</span></span>

<span data-ttu-id="f92df-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f92df-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f92df-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f92df-117">Permission type</span></span>      | <span data-ttu-id="f92df-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f92df-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f92df-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f92df-119">Delegated (work or school account)</span></span> | <span data-ttu-id="f92df-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f92df-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f92df-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f92df-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f92df-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f92df-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f92df-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f92df-123">Application</span></span> | <span data-ttu-id="f92df-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f92df-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f92df-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f92df-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="f92df-126">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f92df-126">Function parameters</span></span>

| <span data-ttu-id="f92df-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f92df-127">Parameter</span></span>   | <span data-ttu-id="f92df-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="f92df-128">Type</span></span>  | <span data-ttu-id="f92df-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="f92df-129">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f92df-130">token</span><span class="sxs-lookup"><span data-stu-id="f92df-130">token</span></span>  | <span data-ttu-id="f92df-131">string</span><span class="sxs-lookup"><span data-stu-id="f92df-131">string</span></span> | <span data-ttu-id="f92df-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f92df-132">Optional.</span></span> <span data-ttu-id="f92df-133">Quando não é especificado, enumera o estado da hierarquia atual.</span><span class="sxs-lookup"><span data-stu-id="f92df-133">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="f92df-134">Quando é `latest`, retorna uma resposta vazia com o token delta mais recente.</span><span class="sxs-lookup"><span data-stu-id="f92df-134">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="f92df-135">Quando é um token delta anterior, retorna o novo estado após o token.</span><span class="sxs-lookup"><span data-stu-id="f92df-135">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="f92df-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f92df-136">Optional query parameters</span></span>

<span data-ttu-id="f92df-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$select`, `$expand` e `$top` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="f92df-137">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="f92df-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f92df-138">Response</span></span>

<span data-ttu-id="f92df-139">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Driveitem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f92df-139">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="f92df-140">Além da coleção de DriveItems, a resposta também incluirá uma das seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="f92df-140">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="f92df-141">Nome</span><span class="sxs-lookup"><span data-stu-id="f92df-141">Name</span></span>                 | <span data-ttu-id="f92df-142">Valor</span><span class="sxs-lookup"><span data-stu-id="f92df-142">Value</span></span>  | <span data-ttu-id="f92df-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="f92df-143">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f92df-144">**\@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="f92df-144">**\@odata.nextLink**</span></span>  | <span data-ttu-id="f92df-145">url</span><span class="sxs-lookup"><span data-stu-id="f92df-145">url</span></span>    | <span data-ttu-id="f92df-146">Uma URL para recuperar a próxima página disponível de alterações, se houver alterações adicionais no conjunto atual.</span><span class="sxs-lookup"><span data-stu-id="f92df-146">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="f92df-147">**\@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="f92df-147">**\@odata.deltaLink**</span></span> | <span data-ttu-id="f92df-148">url</span><span class="sxs-lookup"><span data-stu-id="f92df-148">url</span></span>    | <span data-ttu-id="f92df-p106">Um URL retornado em no lugar de **\@odata.nextLink** após todas as alterações atuais terem sido retornadas. Usado para ler o próximo conjunto de alterações no futuro.</span><span class="sxs-lookup"><span data-stu-id="f92df-p106">A URL returned instead of **\@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="f92df-151">Exemplo (solicitação inicial)</span><span class="sxs-lookup"><span data-stu-id="f92df-151">Example (Initial Request)</span></span>

<span data-ttu-id="f92df-152">Veja a seguir um exemplo de como chamar essa API para estabelecer seu estado local.</span><span class="sxs-lookup"><span data-stu-id="f92df-152">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="f92df-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f92df-153">Request</span></span>

<span data-ttu-id="f92df-154">Veja a seguir um exemplo da solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="f92df-154">Here is an example of the initial request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f92df-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="f92df-155">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_first", "tags": "service.graph" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```
# <a name="c"></a>[<span data-ttu-id="f92df-156">C#</span><span class="sxs-lookup"><span data-stu-id="f92df-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-first-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f92df-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f92df-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-first-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f92df-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f92df-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-first-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f92df-159">Java</span><span class="sxs-lookup"><span data-stu-id="f92df-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-first-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f92df-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="f92df-160">Response</span></span>

<span data-ttu-id="f92df-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f92df-161">Here is an example of the response.</span></span>

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

<span data-ttu-id="f92df-p107">Essa resposta inclui a primeira página de alterações e a propriedade **\@odata.nextLink** indica que há mais itens disponíveis no conjunto atual de itens. Seu aplicativo deve continuar a solicitar o valor de URL de **\@odata.nextLink** até que todas as páginas de itens tenham sido recuperadas.</span><span class="sxs-lookup"><span data-stu-id="f92df-p107">This response includes the first page of changes, and the **\@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **\@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="f92df-164">Exemplo (última página de um conjunto)</span><span class="sxs-lookup"><span data-stu-id="f92df-164">Example (Last page in a set)</span></span>

<span data-ttu-id="f92df-165">Veja a seguir um exemplo de como chamar essa API para atualizar seu estado local.</span><span class="sxs-lookup"><span data-stu-id="f92df-165">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="f92df-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f92df-166">Request</span></span>

<span data-ttu-id="f92df-167">Veja a seguir um exemplo da solicitação após a solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="f92df-167">Here is an example request after the initial request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f92df-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="f92df-168">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-delta-last", "tags": "service.graph" }-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```
# <a name="c"></a>[<span data-ttu-id="f92df-169">C#</span><span class="sxs-lookup"><span data-stu-id="f92df-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-last-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f92df-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f92df-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-last-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f92df-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f92df-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-last-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f92df-172">Java</span><span class="sxs-lookup"><span data-stu-id="f92df-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-last-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f92df-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="f92df-173">Response</span></span>

<span data-ttu-id="f92df-174">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f92df-174">Here is an example of the response.</span></span>

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

<span data-ttu-id="f92df-175">Essa resposta indica que o item denominado `folder2` foi excluído e que o item `file.txt` foi adicionado ou modificado entre a solicitação inicial e essa solicitação para atualizar o estado local.</span><span class="sxs-lookup"><span data-stu-id="f92df-175">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="f92df-176">A página final dos itens incluirá a propriedade **\@odata.deltaLink**, que fornece a URL que pode ser usada posteriormente para recuperar alterações desde o conjunto atual de itens.</span><span class="sxs-lookup"><span data-stu-id="f92df-176">The final page of items will include the **\@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="f92df-p108">Pode haver casos em que o serviço não pode fornecer uma lista de alterações para um determinado token (por exemplo, se um cliente tentar reutilizar um token antigo depois de ter permanecido desconectado por um longo período, ou se o estado do servidor tiver mudado e um novo token for obrigatório). Nesses casos, o serviço retornará um erro `HTTP 410 Gone` com uma resposta de erro contendo um dos códigos de erro abaixo e um cabeçalho `Location` contendo um novo nextLink que inicia uma enumeração delta do zero. Depois de concluir a enumeração completa, compare os itens retornados com seu estado local e siga estas instruções.</span><span class="sxs-lookup"><span data-stu-id="f92df-p108">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="f92df-180">Tipo de erro</span><span class="sxs-lookup"><span data-stu-id="f92df-180">Error Type</span></span>                       | <span data-ttu-id="f92df-181">Instruções</span><span class="sxs-lookup"><span data-stu-id="f92df-181">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="f92df-p109">Substitua todos os itens locais pela versão do servidor (incluindo exclusões) se você tiver certeza de que o serviço estava atualizado com suas alterações locais quando você sincronizou pela última vez. Carregue alterações locais que o servidor não conhece.</span><span class="sxs-lookup"><span data-stu-id="f92df-p109">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="f92df-184">Carregue os itens locais que o serviço não retornou e carregue os arquivos que diferem da versão do servidor (mantendo ambas as cópias se você não tiver certeza de qual é a mais atual).</span><span class="sxs-lookup"><span data-stu-id="f92df-184">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="f92df-185">Recuperar o deltaLink atual</span><span class="sxs-lookup"><span data-stu-id="f92df-185">Retrieving the current deltaLink</span></span>

<span data-ttu-id="f92df-186">Em alguns cenários, pode ser útil solicitar o valor do deltaLink atual sem primeiro enumerar todos os itens que já estão na unidade.</span><span class="sxs-lookup"><span data-stu-id="f92df-186">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="f92df-p110">Isso poderá ser útil se o seu aplicativo quiser apenas saber sobre as alterações e não quiser saber sobre os itens existentes. Para recuperar o deltaLink mais recente, chame `delta` com um parâmetro de cadeia de caracteres de consulta `?token=latest`.</span><span class="sxs-lookup"><span data-stu-id="f92df-p110">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items. To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="f92df-189">**Observação: Se você estiver tentando manter uma representação local completa dos itens em uma pasta ou unidade, use `delta` para a enumeração inicial. Outros métodos, como fazer a paginação por meio da coleção `children` de uma pasta, não garantirá o retorno de todos os itens se ocorrerem gravações durante a enumeração. O uso de `delta` é a única maneira de garantir a leitura de todos os dados necessários.**</span><span class="sxs-lookup"><span data-stu-id="f92df-189">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="f92df-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f92df-190">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f92df-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="f92df-191">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-latest", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```msgraph-interactive
GET /me/drive/root/delta?token=latest
```
# <a name="c"></a>[<span data-ttu-id="f92df-192">C#</span><span class="sxs-lookup"><span data-stu-id="f92df-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-latest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f92df-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f92df-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-latest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f92df-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f92df-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-latest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f92df-195">Java</span><span class="sxs-lookup"><span data-stu-id="f92df-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-latest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f92df-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="f92df-196">Response</span></span>

<!-- { "blockType": "response", "isEmpty": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="f92df-197">Comentários</span><span class="sxs-lookup"><span data-stu-id="f92df-197">Remarks</span></span>

* <span data-ttu-id="f92df-p111">O feed delta mostra o estado mais recente de cada item, e não cada alteração. Se um item tiver sido renomeado duas vezes, ele só aparecerá uma vez, com seu nome mais recente.</span><span class="sxs-lookup"><span data-stu-id="f92df-p111">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="f92df-p112">O mesmo item pode aparecer mais de uma vez em um feed delta, por vários motivos. Você deve usar a última ocorrência que visualizar.</span><span class="sxs-lookup"><span data-stu-id="f92df-p112">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="f92df-p113">A propriedade `parentReference` em itens não incluirá um valor para **path**. Isso ocorre porque a renomeação de uma pasta não faz com que os descendentes dessa pasta sejam retornados de **delta**. **Ao usar delta, você sempre deve controlar itens por id**.</span><span class="sxs-lookup"><span data-stu-id="f92df-p113">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="f92df-205">A consulta delta não retornará algumas propriedades DriveItem, dependendo da operação e do tipo de serviço, conforme mostrado nas tabelas a seguir.</span><span class="sxs-lookup"><span data-stu-id="f92df-205">Delta query will not return some DriveItem properties, depending on the operation and service type, as shown in the following tables.</span></span>

    <span data-ttu-id="f92df-206">**OneDrive for Business**</span><span class="sxs-lookup"><span data-stu-id="f92df-206">**OneDrive for Business**</span></span>
    
    | <span data-ttu-id="f92df-207">Tipo de operação</span><span class="sxs-lookup"><span data-stu-id="f92df-207">Operation type</span></span> | <span data-ttu-id="f92df-208">Propriedades omitidas pela consulta delta</span><span class="sxs-lookup"><span data-stu-id="f92df-208">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="f92df-209">Criar/Modificar</span><span class="sxs-lookup"><span data-stu-id="f92df-209">Create/Modify</span></span> | <span data-ttu-id="f92df-210">`ctag`, `lastModifiedBy`</span><span class="sxs-lookup"><span data-stu-id="f92df-210">`ctag`, `lastModifiedBy`</span></span> |
    | <span data-ttu-id="f92df-211">Excluir</span><span class="sxs-lookup"><span data-stu-id="f92df-211">Delete</span></span> | <span data-ttu-id="f92df-212">`ctag`, `lastModifiedBy`, `name`</span><span class="sxs-lookup"><span data-stu-id="f92df-212">`ctag`, `lastModifiedBy`, `name`</span></span> |


    <span data-ttu-id="f92df-213">**OneDrive (consumidor)**</span><span class="sxs-lookup"><span data-stu-id="f92df-213">**OneDrive (consumer)**</span></span>
    
    | <span data-ttu-id="f92df-214">Tipo de operação</span><span class="sxs-lookup"><span data-stu-id="f92df-214">Operation type</span></span> | <span data-ttu-id="f92df-215">Propriedades omitidas pela consulta delta</span><span class="sxs-lookup"><span data-stu-id="f92df-215">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="f92df-216">Criar/Modificar</span><span class="sxs-lookup"><span data-stu-id="f92df-216">Create/Modify</span></span> | <span data-ttu-id="f92df-217">n/d</span><span class="sxs-lookup"><span data-stu-id="f92df-217">n/a</span></span> |
    | <span data-ttu-id="f92df-218">Excluir</span><span class="sxs-lookup"><span data-stu-id="f92df-218">Delete</span></span> | <span data-ttu-id="f92df-219">`ctag`, `size`</span><span class="sxs-lookup"><span data-stu-id="f92df-219">`ctag`, `size`</span></span> |

## <a name="scanning-permissions-hierarchies"></a><span data-ttu-id="f92df-220">Hierarquias de permissões de verificação</span><span class="sxs-lookup"><span data-stu-id="f92df-220">Scanning permissions hierarchies</span></span>
<span data-ttu-id="f92df-221">Por padrão, a resposta da consulta delta incluirá o compartilhamento de informações de todos os itens da consulta que foram alterados, mesmo que herdem suas permissões dos pais e não tenham elas próprias alterações diretas de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="f92df-221">By default, the delta query response will include sharing information for all items in the query that changed even if they inherit their permissions from their parent and did not have direct sharing changes themselves.</span></span> <span data-ttu-id="f92df-222">Isso normalmente resulta em uma chamada de acompanhamento para obter os detalhes da permissão de cada item, e não apenas daqueles cujas informações de compartilhamento foram alteradas.</span><span class="sxs-lookup"><span data-stu-id="f92df-222">This typically then results in a follow up call to get the permission details for every item rather than just the ones whose sharing information changed.</span></span> <span data-ttu-id="f92df-223">Você pode otimizar sua compreensão de como as alterações de permissão acontecem adicionando o cabeçalho `Prefer: hierarchicalsharing` à sua solicitação de consulta delta.</span><span class="sxs-lookup"><span data-stu-id="f92df-223">You can optimize your understanding of how permission changes happen by adding the `Prefer: hierarchicalsharing` header to your delta query request.</span></span>

<span data-ttu-id="f92df-224">Quando o cabeçalho `Prefer: hierarchicalsharing` é fornecido, as informações de compartilhamento serão retornadas para a raiz da hierarquia de permissões, bem como itens que possuam, explicitamente, alterações de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="f92df-224">When the `Prefer: hierarchicalsharing` header is provided, sharing information will be returned for the root of the permissions hierarchy, as well as items that explicitly have sharing changes.</span></span> <span data-ttu-id="f92df-225">Nos casos onde a mudança de compartilhamento é remover o compartilhamento de um item, você encontrará uma faceta de compartilhamento vazia para diferenciar entre os itens que herdam de seus pais e aqueles que são únicos, mas sem links de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="f92df-225">In cases where the sharing change is to remove sharing from an item, you will find an empty sharing facet to differentiate between items that inherit from their parent and those that are unique but have no sharing links.</span></span> <span data-ttu-id="f92df-226">Você também verá essa faceta de compartilhamento vazia na raiz de uma hierarquia de permissões que não é compartilhada para estabelecer o escopo inicial.</span><span class="sxs-lookup"><span data-stu-id="f92df-226">You will also see this empty sharing facet on the root of a permission hierarchy that is not shared to establish the initial scope.</span></span>

<span data-ttu-id="f92df-227">Em muitos cenários de verificação, você pode estar interessado, especificamente, em alterações nas permissões.</span><span class="sxs-lookup"><span data-stu-id="f92df-227">In many scanning scenarios, you might be interested specifically in changes to permissions.</span></span> <span data-ttu-id="f92df-228">Para deixar claro na resposta da consulta delta quais alterações são resultados de alterações nas permissões, você pode fornecer o cabeçalho `Prefer: deltashowsharingchanges`.</span><span class="sxs-lookup"><span data-stu-id="f92df-228">To make it clear in the delta query response which changes are the result of permissions being changed, you can provide the `Prefer: deltashowsharingchanges` header.</span></span> <span data-ttu-id="f92df-229">Quando esse cabeçalho é fornecido, todos os itens que aparecem na resposta da consulta delta devido a alterações de permissão, terão a anotação OData `@microsoft.graph.sharedChanged":"True"`.</span><span class="sxs-lookup"><span data-stu-id="f92df-229">When this header is provided, all items that appear in the delta query response due to permission changes will have the `@microsoft.graph.sharedChanged":"True"` OData annotation.</span></span> <span data-ttu-id="f92df-230">Esse recurso é aplicável ao SharePoint e ao OneDrive for Business, mas não às contas de consumidor do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f92df-230">This feature is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

> <span data-ttu-id="f92df-231">**Nota:** O uso do cabeçalho `Prefer: deltashowsharingchanges` requer que você use `Prefer: deltashowremovedasdeleted` e `Prefer: deltatraversepermissiongaps`.</span><span class="sxs-lookup"><span data-stu-id="f92df-231">**Note:** The use of `Prefer: deltashowsharingchanges` header requires you to use `Prefer: deltashowremovedasdeleted` and `Prefer: deltatraversepermissiongaps`.</span></span> <span data-ttu-id="f92df-232">Esses valores de cabeçalho podem ser agrupados em um único cabeçalho: `Prefer: deltashowremovedasdeleted, deltatraversepermissiongaps, deltashowsharingchanges`.</span><span class="sxs-lookup"><span data-stu-id="f92df-232">These header values can be joined together in a single header: `Prefer: deltashowremovedasdeleted, deltatraversepermissiongaps, deltashowsharingchanges`.</span></span>

## <a name="error-responses"></a><span data-ttu-id="f92df-233">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="f92df-233">Error responses</span></span>

<span data-ttu-id="f92df-234">Além dos erros de ressincronização detalhados acima, confira os detalhes sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="f92df-234">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

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

