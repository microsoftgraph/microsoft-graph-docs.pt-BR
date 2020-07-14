---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Sincronizar o conteúdo de uma unidade
localization_priority: Priority
ms.prod: sharepoint
description: Esse método permite que o seu aplicativo controle alterações em uma unidade e seus filhos com o passar do tempo.
doc_type: apiPageType
ms.openlocfilehash: d86a02efc98d604bb970faea07c058e3a8651bfa
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038685"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="c774d-103">Controlar alterações para uma unidade</span><span class="sxs-lookup"><span data-stu-id="c774d-103">Track changes for a Drive</span></span>

<span data-ttu-id="c774d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c774d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c774d-105">Esse método permite que o seu aplicativo controle alterações em uma unidade e seus filhos com o passar do tempo.</span><span class="sxs-lookup"><span data-stu-id="c774d-105">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="c774d-106">Your app begins by calling `delta` without any parameters.</span><span class="sxs-lookup"><span data-stu-id="c774d-106">Your app begins by calling `delta` without any parameters.</span></span> <span data-ttu-id="c774d-107">The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below.</span><span class="sxs-lookup"><span data-stu-id="c774d-107">The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below.</span></span>
<span data-ttu-id="c774d-108">Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span><span class="sxs-lookup"><span data-stu-id="c774d-108">Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="c774d-109">After you have finished receiving all the changes, you may apply them to your local state.</span><span class="sxs-lookup"><span data-stu-id="c774d-109">After you have finished receiving all the changes, you may apply them to your local state.</span></span>
<span data-ttu-id="c774d-110">To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span><span class="sxs-lookup"><span data-stu-id="c774d-110">To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="c774d-111">Deleted items are returned with the [`deleted` facet](../resources/deleted.md).</span><span class="sxs-lookup"><span data-stu-id="c774d-111">Deleted items are returned with the [`deleted` facet](../resources/deleted.md).</span></span> <span data-ttu-id="c774d-112">Items with this property set should be removed from your local state.</span><span class="sxs-lookup"><span data-stu-id="c774d-112">Items with this property set should be removed from your local state.</span></span> 

><span data-ttu-id="c774d-113">**Observação:** você apenas deverá excluir uma pasta localmente se ela ficar vazia após a sincronização de todas as alterações.</span><span class="sxs-lookup"><span data-stu-id="c774d-113">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="c774d-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="c774d-114">Permissions</span></span>

<span data-ttu-id="c774d-115">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c774d-115">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c774d-116">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c774d-116">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c774d-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c774d-117">Permission type</span></span>      | <span data-ttu-id="c774d-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c774d-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c774d-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c774d-119">Delegated (work or school account)</span></span> | <span data-ttu-id="c774d-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c774d-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c774d-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c774d-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c774d-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c774d-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c774d-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c774d-123">Application</span></span> | <span data-ttu-id="c774d-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c774d-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c774d-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c774d-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="c774d-126">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c774d-126">Function parameters</span></span>

| <span data-ttu-id="c774d-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c774d-127">Parameter</span></span>   | <span data-ttu-id="c774d-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="c774d-128">Type</span></span>  | <span data-ttu-id="c774d-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c774d-129">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c774d-130">token</span><span class="sxs-lookup"><span data-stu-id="c774d-130">token</span></span>  | <span data-ttu-id="c774d-131">string</span><span class="sxs-lookup"><span data-stu-id="c774d-131">string</span></span> | <span data-ttu-id="c774d-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c774d-132">Optional.</span></span> <span data-ttu-id="c774d-133">Quando não é especificado, enumera o estado da hierarquia atual.</span><span class="sxs-lookup"><span data-stu-id="c774d-133">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="c774d-134">Quando é `latest`, retorna uma resposta vazia com o token delta mais recente.</span><span class="sxs-lookup"><span data-stu-id="c774d-134">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="c774d-135">Quando é um token delta anterior, retorna o novo estado após o token.</span><span class="sxs-lookup"><span data-stu-id="c774d-135">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c774d-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c774d-136">Optional query parameters</span></span>

<span data-ttu-id="c774d-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$select`, `$expand` e `$top` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="c774d-137">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="c774d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c774d-138">Response</span></span>

<span data-ttu-id="c774d-139">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Driveitem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c774d-139">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="c774d-140">Além da coleção de DriveItems, a resposta também incluirá uma das seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="c774d-140">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="c774d-141">Nome</span><span class="sxs-lookup"><span data-stu-id="c774d-141">Name</span></span>                 | <span data-ttu-id="c774d-142">Valor</span><span class="sxs-lookup"><span data-stu-id="c774d-142">Value</span></span>  | <span data-ttu-id="c774d-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="c774d-143">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c774d-144">**\@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="c774d-144">**\@odata.nextLink**</span></span>  | <span data-ttu-id="c774d-145">url</span><span class="sxs-lookup"><span data-stu-id="c774d-145">url</span></span>    | <span data-ttu-id="c774d-146">Uma URL para recuperar a próxima página disponível de alterações, se houver alterações adicionais no conjunto atual.</span><span class="sxs-lookup"><span data-stu-id="c774d-146">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="c774d-147">**\@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="c774d-147">**\@odata.deltaLink**</span></span> | <span data-ttu-id="c774d-148">url</span><span class="sxs-lookup"><span data-stu-id="c774d-148">url</span></span>    | <span data-ttu-id="c774d-149">Uma URL retornada em vez de **\@odata.nextLink** após o retorno de todas as alterações atuais.</span><span class="sxs-lookup"><span data-stu-id="c774d-149">A URL returned instead of **\@odata.nextLink** after all current changes have been returned.</span></span> <span data-ttu-id="c774d-150">Usada para ler o próximo conjunto de alterações no futuro.</span><span class="sxs-lookup"><span data-stu-id="c774d-150">Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="c774d-151">Exemplo (solicitação inicial)</span><span class="sxs-lookup"><span data-stu-id="c774d-151">Example (Initial Request)</span></span>

<span data-ttu-id="c774d-152">Veja a seguir um exemplo de como chamar essa API para estabelecer seu estado local.</span><span class="sxs-lookup"><span data-stu-id="c774d-152">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="c774d-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c774d-153">Request</span></span>

<span data-ttu-id="c774d-154">Veja a seguir um exemplo da solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="c774d-154">Here is an example of the initial request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c774d-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="c774d-155">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_first", "tags": "service.graph" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```
# <a name="c"></a>[<span data-ttu-id="c774d-156">C#</span><span class="sxs-lookup"><span data-stu-id="c774d-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-first-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c774d-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c774d-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-first-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c774d-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c774d-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-first-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c774d-159">Java</span><span class="sxs-lookup"><span data-stu-id="c774d-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-first-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c774d-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="c774d-160">Response</span></span>

<span data-ttu-id="c774d-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c774d-161">Here is an example of the response.</span></span>

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

<span data-ttu-id="c774d-162">Essa resposta inclui a primeira página de alterações e a propriedade **\@odata.nextLink** indica que há mais itens disponíveis no conjunto atual de itens.</span><span class="sxs-lookup"><span data-stu-id="c774d-162">This response includes the first page of changes, and the **\@odata.nextLink** property indicates that there are more items available in the current set of items.</span></span>
<span data-ttu-id="c774d-163">Seu aplicativo deve continuar solicitando o valor da URL **\@odata.nextLink** até que todas as páginas de itens tenham sido recuperadas.</span><span class="sxs-lookup"><span data-stu-id="c774d-163">Your app should continue to request the URL value of **\@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="c774d-164">Exemplo (última página de um conjunto)</span><span class="sxs-lookup"><span data-stu-id="c774d-164">Example (Last page in a set)</span></span>

<span data-ttu-id="c774d-165">Veja a seguir um exemplo de como chamar essa API para atualizar seu estado local.</span><span class="sxs-lookup"><span data-stu-id="c774d-165">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="c774d-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c774d-166">Request</span></span>

<span data-ttu-id="c774d-167">Veja a seguir um exemplo da solicitação após a solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="c774d-167">Here is an example request after the initial request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c774d-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="c774d-168">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-delta-last", "tags": "service.graph" }-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```
# <a name="c"></a>[<span data-ttu-id="c774d-169">C#</span><span class="sxs-lookup"><span data-stu-id="c774d-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-last-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c774d-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c774d-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-last-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c774d-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c774d-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-last-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c774d-172">Java</span><span class="sxs-lookup"><span data-stu-id="c774d-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-last-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c774d-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="c774d-173">Response</span></span>

<span data-ttu-id="c774d-174">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c774d-174">Here is an example of the response.</span></span>

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

<span data-ttu-id="c774d-175">Essa resposta indica que o item denominado `folder2` foi excluído e que o item `file.txt` foi adicionado ou modificado entre a solicitação inicial e essa solicitação para atualizar o estado local.</span><span class="sxs-lookup"><span data-stu-id="c774d-175">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="c774d-176">A página final dos itens incluirá a propriedade **\@odata.deltaLink**, que fornece a URL que pode ser usada posteriormente para recuperar alterações desde o conjunto atual de itens.</span><span class="sxs-lookup"><span data-stu-id="c774d-176">The final page of items will include the **\@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="c774d-177">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required).</span><span class="sxs-lookup"><span data-stu-id="c774d-177">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required).</span></span>
<span data-ttu-id="c774d-178">In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch.</span><span class="sxs-lookup"><span data-stu-id="c774d-178">In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch.</span></span>
<span data-ttu-id="c774d-179">After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span><span class="sxs-lookup"><span data-stu-id="c774d-179">After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="c774d-180">Tipo de erro</span><span class="sxs-lookup"><span data-stu-id="c774d-180">Error Type</span></span>                       | <span data-ttu-id="c774d-181">Instruções</span><span class="sxs-lookup"><span data-stu-id="c774d-181">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="c774d-182">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd.</span><span class="sxs-lookup"><span data-stu-id="c774d-182">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd.</span></span> <span data-ttu-id="c774d-183">Upload any local changes that the server doesn't know about.</span><span class="sxs-lookup"><span data-stu-id="c774d-183">Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="c774d-184">Carregue os itens locais que o serviço não retornou e carregue os arquivos que diferem da versão do servidor (mantendo ambas as cópias se você não tiver certeza de qual é a mais atual).</span><span class="sxs-lookup"><span data-stu-id="c774d-184">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="c774d-185">Recuperar o deltaLink atual</span><span class="sxs-lookup"><span data-stu-id="c774d-185">Retrieving the current deltaLink</span></span>

<span data-ttu-id="c774d-186">Em alguns cenários, pode ser útil solicitar o valor do deltaLink atual sem primeiro enumerar todos os itens que já estão na unidade.</span><span class="sxs-lookup"><span data-stu-id="c774d-186">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="c774d-187">Isso poderá ser útil se o seu aplicativo quiser saber apenas sobre as alterações, e não quiser saber sobre os itens existentes.</span><span class="sxs-lookup"><span data-stu-id="c774d-187">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items.</span></span>
<span data-ttu-id="c774d-188">Para recuperar o deltaLink mais recente, chame `delta` com um parâmetro de cadeia de caracteres de consulta `?token=latest`.</span><span class="sxs-lookup"><span data-stu-id="c774d-188">To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="c774d-189">**Observação: Se você estiver tentando manter uma representação local completa dos itens em uma pasta ou unidade, use `delta` para a enumeração inicial. Outros métodos, como fazer a paginação por meio da coleção `children` de uma pasta, não garantirá o retorno de todos os itens se ocorrerem gravações durante a enumeração. O uso de `delta` é a única maneira de garantir a leitura de todos os dados necessários.**</span><span class="sxs-lookup"><span data-stu-id="c774d-189">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="c774d-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c774d-190">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c774d-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="c774d-191">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-latest", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```msgraph-interactive
GET /me/drive/root/delta?token=latest
```
# <a name="c"></a>[<span data-ttu-id="c774d-192">C#</span><span class="sxs-lookup"><span data-stu-id="c774d-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-latest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c774d-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c774d-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-latest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c774d-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c774d-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-latest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c774d-195">Java</span><span class="sxs-lookup"><span data-stu-id="c774d-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-latest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c774d-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="c774d-196">Response</span></span>

<!-- { "blockType": "response", "isEmpty": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="c774d-197">Comentários</span><span class="sxs-lookup"><span data-stu-id="c774d-197">Remarks</span></span>

* <span data-ttu-id="c774d-198">The delta feed shows the latest state for each item, not each change.</span><span class="sxs-lookup"><span data-stu-id="c774d-198">The delta feed shows the latest state for each item, not each change.</span></span> <span data-ttu-id="c774d-199">If an item were renamed twice, it would only show up once, with its latest name.</span><span class="sxs-lookup"><span data-stu-id="c774d-199">If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="c774d-200">The same item may appear more than once in a delta feed, for various reasons.</span><span class="sxs-lookup"><span data-stu-id="c774d-200">The same item may appear more than once in a delta feed, for various reasons.</span></span> <span data-ttu-id="c774d-201">You should use the last occurrence you see.</span><span class="sxs-lookup"><span data-stu-id="c774d-201">You should use the last occurrence you see.</span></span>
* <span data-ttu-id="c774d-202">The `parentReference` property on items will not include a value for **path**.</span><span class="sxs-lookup"><span data-stu-id="c774d-202">The `parentReference` property on items will not include a value for **path**.</span></span> <span data-ttu-id="c774d-203">This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**.</span><span class="sxs-lookup"><span data-stu-id="c774d-203">This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**.</span></span> <span data-ttu-id="c774d-204">**When using delta you should always track items by id**.</span><span class="sxs-lookup"><span data-stu-id="c774d-204">**When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="c774d-205">No OneDrive for Business e no SharePoint, `delta` tem suporte apenas na pasta `root`, e não em outras pastas dentro de uma unidade.</span><span class="sxs-lookup"><span data-stu-id="c774d-205">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders within a drive.</span></span>

* <span data-ttu-id="c774d-206">A consulta delta não retornará algumas propriedades DriveItem, dependendo da operação e do tipo de serviço, conforme mostrado nas tabelas a seguir.</span><span class="sxs-lookup"><span data-stu-id="c774d-206">Delta query will not return some DriveItem properties, depending on the operation and service type, as shown in the following tables.</span></span>

    <span data-ttu-id="c774d-207">**OneDrive for Business**</span><span class="sxs-lookup"><span data-stu-id="c774d-207">**OneDrive for Business**</span></span>
    
    | <span data-ttu-id="c774d-208">Tipo de operação</span><span class="sxs-lookup"><span data-stu-id="c774d-208">Operation type</span></span> | <span data-ttu-id="c774d-209">Propriedades omitidas pela consulta delta</span><span class="sxs-lookup"><span data-stu-id="c774d-209">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="c774d-210">Criar/Modificar</span><span class="sxs-lookup"><span data-stu-id="c774d-210">Create/Modify</span></span> | <span data-ttu-id="c774d-211">`ctag`, `lastModifiedBy`</span><span class="sxs-lookup"><span data-stu-id="c774d-211">`ctag`, `lastModifiedBy`</span></span> |
    | <span data-ttu-id="c774d-212">Excluir</span><span class="sxs-lookup"><span data-stu-id="c774d-212">Delete</span></span> | <span data-ttu-id="c774d-213">`ctag`, `lastModifiedBy`, `name`</span><span class="sxs-lookup"><span data-stu-id="c774d-213">`ctag`, `lastModifiedBy`, `name`</span></span> |


    <span data-ttu-id="c774d-214">**OneDrive (consumidor)**</span><span class="sxs-lookup"><span data-stu-id="c774d-214">**OneDrive (consumer)**</span></span>
    
    | <span data-ttu-id="c774d-215">Tipo de operação</span><span class="sxs-lookup"><span data-stu-id="c774d-215">Operation type</span></span> | <span data-ttu-id="c774d-216">Propriedades omitidas pela consulta delta</span><span class="sxs-lookup"><span data-stu-id="c774d-216">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="c774d-217">Criar/Modificar</span><span class="sxs-lookup"><span data-stu-id="c774d-217">Create/Modify</span></span> | <span data-ttu-id="c774d-218">n/d</span><span class="sxs-lookup"><span data-stu-id="c774d-218">n/a</span></span> |
    | <span data-ttu-id="c774d-219">Excluir</span><span class="sxs-lookup"><span data-stu-id="c774d-219">Delete</span></span> | <span data-ttu-id="c774d-220">`ctag`, `size`</span><span class="sxs-lookup"><span data-stu-id="c774d-220">`ctag`, `size`</span></span> |

## <a name="scanning-permissions-hierarchies"></a><span data-ttu-id="c774d-221">Hierarquias de permissões de verificação</span><span class="sxs-lookup"><span data-stu-id="c774d-221">Scanning permissions hierarchies</span></span>
<span data-ttu-id="c774d-222">Por padrão, a resposta da consulta delta incluirá o compartilhamento de informações de todos os itens da consulta que foram alterados, mesmo que herdem suas permissões dos pais e não tenham elas próprias alterações diretas de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="c774d-222">By default, the delta query response will include sharing information for all items in the query that changed even if they inherit their permissions from their parent and did not have direct sharing changes themselves.</span></span> <span data-ttu-id="c774d-223">Isso normalmente resulta em uma chamada de acompanhamento para obter os detalhes da permissão de cada item, e não apenas daqueles cujas informações de compartilhamento foram alteradas.</span><span class="sxs-lookup"><span data-stu-id="c774d-223">This typically then results in a follow up call to get the permission details for every item rather than just the ones whose sharing information changed.</span></span> <span data-ttu-id="c774d-224">Você pode otimizar sua compreensão de como as alterações de permissão acontecem adicionando o cabeçalho `Prefer: hierarchicalsharing` à sua solicitação de consulta delta.</span><span class="sxs-lookup"><span data-stu-id="c774d-224">You can optimize your understanding of how permission changes happen by adding the `Prefer: hierarchicalsharing` header to your delta query request.</span></span>

<span data-ttu-id="c774d-225">Quando o cabeçalho `Prefer: hierarchicalsharing` é fornecido, as informações de compartilhamento serão retornadas para a raiz da hierarquia de permissões, bem como itens que possuam, explicitamente, alterações de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="c774d-225">When the `Prefer: hierarchicalsharing` header is provided, sharing information will be returned for the root of the permissions hierarchy, as well as items that explicitly have sharing changes.</span></span> <span data-ttu-id="c774d-226">Nos casos onde a mudança de compartilhamento é remover o compartilhamento de um item, você encontrará uma faceta de compartilhamento vazia para diferenciar entre os itens que herdam de seus pais e aqueles que são únicos, mas sem links de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="c774d-226">In cases where the sharing change is to remove sharing from an item, you will find an empty sharing facet to differentiate between items that inherit from their parent and those that are unique but have no sharing links.</span></span> <span data-ttu-id="c774d-227">Você também verá essa faceta de compartilhamento vazia na raiz de uma hierarquia de permissões que não é compartilhada para estabelecer o escopo inicial.</span><span class="sxs-lookup"><span data-stu-id="c774d-227">You will also see this empty sharing facet on the root of a permission hierarchy that is not shared to establish the initial scope.</span></span>

<span data-ttu-id="c774d-228">Em muitos cenários de verificação, você pode estar interessado, especificamente, em alterações nas permissões.</span><span class="sxs-lookup"><span data-stu-id="c774d-228">In many scanning scenarios, you might be interested specifically in changes to permissions.</span></span> <span data-ttu-id="c774d-229">Para deixar claro na resposta da consulta delta quais alterações são resultados de alterações nas permissões, você pode fornecer o cabeçalho `Prefer: deltashowsharingchanges`.</span><span class="sxs-lookup"><span data-stu-id="c774d-229">To make it clear in the delta query response which changes are the result of permissions being changed, you can provide the `Prefer: deltashowsharingchanges` header.</span></span> <span data-ttu-id="c774d-230">Quando esse cabeçalho é fornecido, todos os itens que aparecem na resposta da consulta delta devido a alterações de permissão, terão a anotação OData `@microsoft.graph.sharedChanged":"True"`.</span><span class="sxs-lookup"><span data-stu-id="c774d-230">When this header is provided, all items that appear in the delta query response due to permission changes will have the `@microsoft.graph.sharedChanged":"True"` OData annotation.</span></span> <span data-ttu-id="c774d-231">Esse recurso é aplicável ao SharePoint e ao OneDrive for Business, mas não às contas de consumidor do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c774d-231">This feature is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

> <span data-ttu-id="c774d-232">**Nota:** O uso do cabeçalho `Prefer: deltashowsharingchanges` requer que você use `Prefer: deltashowremovedasdeleted` e `Prefer: deltatraversepermissiongaps`.</span><span class="sxs-lookup"><span data-stu-id="c774d-232">**Note:** The use of `Prefer: deltashowsharingchanges` header requires you to use `Prefer: deltashowremovedasdeleted` and `Prefer: deltatraversepermissiongaps`.</span></span> <span data-ttu-id="c774d-233">Esses valores de cabeçalho podem ser combinados em um único cabeçalho: `Prefer: deltashowremovedasdeleted; deltatraversepermissiongaps; deltashowsharingchanges;`.</span><span class="sxs-lookup"><span data-stu-id="c774d-233">These header values can be joint together in a single header: `Prefer: deltashowremovedasdeleted; deltatraversepermissiongaps; deltashowsharingchanges;`.</span></span>

## <a name="error-responses"></a><span data-ttu-id="c774d-234">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="c774d-234">Error responses</span></span>

<span data-ttu-id="c774d-235">Além dos erros de ressincronização detalhados acima, confira os detalhes sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="c774d-235">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

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
