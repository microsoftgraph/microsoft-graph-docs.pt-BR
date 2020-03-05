---
author: JeremyKelley
description: Esse método permite que o seu aplicativo controle alterações em uma unidade e seus filhos com o passar do tempo.
ms.date: 09/10/2017
title: Sincronizar o conteúdo de uma unidade
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a8cbbff6eaada0730ee5a70a982e053388ded817
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432779"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="494c8-103">Controlar alterações para uma unidade</span><span class="sxs-lookup"><span data-stu-id="494c8-103">Track changes for a Drive</span></span>

<span data-ttu-id="494c8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="494c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="494c8-105">Esse método permite que o seu aplicativo controle alterações em uma unidade e seus filhos com o passar do tempo.</span><span class="sxs-lookup"><span data-stu-id="494c8-105">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="494c8-p101">Seu aplicativo começa chamando `delta` sem parâmetros. O serviço começa a enumerar a hierarquia da unidade, retornando páginas de itens e um `@odata.nextLink` ou `@odata.deltaLink`, conforme descrito abaixo. Seu aplicativo deve continuar chamando com o `@odata.nextLink` até que você não veja mais um `@odata.nextLink` retornado ou até que você veja uma resposta com um conjunto vazio de alterações.</span><span class="sxs-lookup"><span data-stu-id="494c8-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="494c8-p102">Quando terminar de receber todas as alterações, você pode aplicá-las ao seu estado local. Para verificar se há alterações no futuro, chame `delta` novamente com o `@odata.deltaLink` da resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="494c8-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="494c8-p103">Itens excluídos são retornados com a [faceta `deleted`](../resources/deleted.md). Itens com esse conjunto de propriedades devem ser removidos do seu estado local.</span><span class="sxs-lookup"><span data-stu-id="494c8-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="494c8-113">**Observação:** você apenas deverá excluir uma pasta localmente se ela ficar vazia após a sincronização de todas as alterações.</span><span class="sxs-lookup"><span data-stu-id="494c8-113">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="494c8-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="494c8-114">Permissions</span></span>

<span data-ttu-id="494c8-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="494c8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="494c8-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="494c8-117">Permission type</span></span>      | <span data-ttu-id="494c8-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="494c8-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="494c8-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="494c8-119">Delegated (work or school account)</span></span> | <span data-ttu-id="494c8-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="494c8-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="494c8-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="494c8-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="494c8-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="494c8-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="494c8-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="494c8-123">Application</span></span> | <span data-ttu-id="494c8-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="494c8-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="494c8-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="494c8-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="494c8-126">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="494c8-126">Function parameters</span></span>

| <span data-ttu-id="494c8-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="494c8-127">Parameter</span></span>   | <span data-ttu-id="494c8-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="494c8-128">Type</span></span>  | <span data-ttu-id="494c8-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="494c8-129">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="494c8-130">token</span><span class="sxs-lookup"><span data-stu-id="494c8-130">token</span></span>  | <span data-ttu-id="494c8-131">string</span><span class="sxs-lookup"><span data-stu-id="494c8-131">string</span></span> | <span data-ttu-id="494c8-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="494c8-132">Optional.</span></span> <span data-ttu-id="494c8-133">Quando não é especificado, enumera o estado da hierarquia atual.</span><span class="sxs-lookup"><span data-stu-id="494c8-133">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="494c8-134">Quando é `latest`, retorna uma resposta vazia com o token delta mais recente.</span><span class="sxs-lookup"><span data-stu-id="494c8-134">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="494c8-135">Quando é um token delta anterior, retorna o novo estado após o token.</span><span class="sxs-lookup"><span data-stu-id="494c8-135">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="494c8-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="494c8-136">Optional query parameters</span></span>

<span data-ttu-id="494c8-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$select`, `$expand` e `$top` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="494c8-137">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="494c8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="494c8-138">Response</span></span>

<span data-ttu-id="494c8-139">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Driveitem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="494c8-139">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="494c8-140">Além da coleção de DriveItems, a resposta também incluirá uma das seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="494c8-140">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="494c8-141">Nome</span><span class="sxs-lookup"><span data-stu-id="494c8-141">Name</span></span>                 | <span data-ttu-id="494c8-142">Valor</span><span class="sxs-lookup"><span data-stu-id="494c8-142">Value</span></span>  | <span data-ttu-id="494c8-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="494c8-143">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="494c8-144">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="494c8-144">**@odata.nextLink**</span></span>  | <span data-ttu-id="494c8-145">url</span><span class="sxs-lookup"><span data-stu-id="494c8-145">url</span></span>    | <span data-ttu-id="494c8-146">Uma URL para recuperar a próxima página disponível de alterações, se houver alterações adicionais no conjunto atual.</span><span class="sxs-lookup"><span data-stu-id="494c8-146">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="494c8-147">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="494c8-147">**@odata.deltaLink**</span></span> | <span data-ttu-id="494c8-148">url</span><span class="sxs-lookup"><span data-stu-id="494c8-148">url</span></span>    | <span data-ttu-id="494c8-p106">Uma URL retornada no lugar de **@odata.nextLink** após o retorno de todas as alterações atuais. Usada para ler o próximo conjunto de alterações no futuro.</span><span class="sxs-lookup"><span data-stu-id="494c8-p106">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="494c8-151">Exemplo (solicitação inicial)</span><span class="sxs-lookup"><span data-stu-id="494c8-151">Example (Initial Request)</span></span>

<span data-ttu-id="494c8-152">Veja a seguir um exemplo de como chamar essa API para estabelecer seu estado local.</span><span class="sxs-lookup"><span data-stu-id="494c8-152">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="494c8-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="494c8-153">Request</span></span>

<span data-ttu-id="494c8-154">Veja a seguir um exemplo da solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="494c8-154">Here is an example of the initial request.</span></span>


# <a name="http"></a>[<span data-ttu-id="494c8-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="494c8-155">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_first" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/root/delta
```
# <a name="c"></a>[<span data-ttu-id="494c8-156">C#</span><span class="sxs-lookup"><span data-stu-id="494c8-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-first-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="494c8-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="494c8-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-first-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="494c8-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="494c8-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-first-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="494c8-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="494c8-159">Response</span></span>

<span data-ttu-id="494c8-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="494c8-160">Here is an example of the response.</span></span>

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

<span data-ttu-id="494c8-p107">Essa resposta inclui a primeira página de alterações, e a propriedade **@odata.nextLink** indica que há mais itens disponíveis no conjunto atual de itens. Seu aplicativo deve continuar a solicitar o valor de URL de **@odata.nextLink** até que todas as páginas de itens tenham sido recuperadas.</span><span class="sxs-lookup"><span data-stu-id="494c8-p107">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="494c8-163">Exemplo (última página de um conjunto)</span><span class="sxs-lookup"><span data-stu-id="494c8-163">Example (Last page in a set)</span></span>

<span data-ttu-id="494c8-164">Veja a seguir um exemplo de como chamar essa API para atualizar seu estado local.</span><span class="sxs-lookup"><span data-stu-id="494c8-164">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="494c8-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="494c8-165">Request</span></span>

<span data-ttu-id="494c8-166">Veja a seguir um exemplo da solicitação após a solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="494c8-166">Here is an example request after the initial request.</span></span>


# <a name="http"></a>[<span data-ttu-id="494c8-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="494c8-167">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_last" }-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/root/delta(token='1230919asd190410jlka')
```
# <a name="c"></a>[<span data-ttu-id="494c8-168">C#</span><span class="sxs-lookup"><span data-stu-id="494c8-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-last-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="494c8-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="494c8-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-last-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="494c8-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="494c8-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-last-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="494c8-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="494c8-171">Response</span></span>

<span data-ttu-id="494c8-172">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="494c8-172">Here is an example of the response.</span></span>

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

<span data-ttu-id="494c8-173">Essa resposta indica que o item denominado `folder2` foi excluído e que o item `file.txt` foi adicionado ou modificado entre a solicitação inicial e essa solicitação para atualizar o estado local.</span><span class="sxs-lookup"><span data-stu-id="494c8-173">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="494c8-174">A página final de itens incluirá a propriedade **@odata.deltaLink**, que fornece a URL que poderá ser usada posteriormente para recuperar alterações desde o conjunto atual de itens.</span><span class="sxs-lookup"><span data-stu-id="494c8-174">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="494c8-p108">Pode haver casos em que o serviço não pode fornecer uma lista de alterações para um determinado token (por exemplo, se um cliente tentar reutilizar um token antigo depois de ter permanecido desconectado por um longo período, ou se o estado do servidor tiver mudado e um novo token for obrigatório). Nesses casos, o serviço retornará um erro `HTTP 410 Gone` com uma resposta de erro contendo um dos códigos de erro abaixo e um cabeçalho `Location` contendo um novo nextLink que inicia uma enumeração delta do zero. Depois de concluir a enumeração completa, compare os itens retornados com seu estado local e siga estas instruções.</span><span class="sxs-lookup"><span data-stu-id="494c8-p108">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="494c8-178">Tipo de erro</span><span class="sxs-lookup"><span data-stu-id="494c8-178">Error Type</span></span>                       | <span data-ttu-id="494c8-179">Instruções</span><span class="sxs-lookup"><span data-stu-id="494c8-179">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="494c8-p109">Substitua todos os itens locais pela versão do servidor (incluindo exclusões) se você tiver certeza de que o serviço estava atualizado com suas alterações locais quando você sincronizou pela última vez. Carregue alterações locais que o servidor não conhece.</span><span class="sxs-lookup"><span data-stu-id="494c8-p109">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="494c8-182">Carregue os itens locais que o serviço não retornou e carregue os arquivos que diferem da versão do servidor (mantendo ambas as cópias se você não tiver certeza de qual é a mais atual).</span><span class="sxs-lookup"><span data-stu-id="494c8-182">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="494c8-183">Recuperar o deltaLink atual</span><span class="sxs-lookup"><span data-stu-id="494c8-183">Retrieving the current deltaLink</span></span>

<span data-ttu-id="494c8-184">Em alguns cenários, pode ser útil solicitar o valor do deltaLink atual sem primeiro enumerar todos os itens que já estão na unidade.</span><span class="sxs-lookup"><span data-stu-id="494c8-184">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="494c8-185">Isso poderá ser útil se o seu aplicativo quiser saber apenas sobre as alterações, e não quiser saber sobre os itens existentes.</span><span class="sxs-lookup"><span data-stu-id="494c8-185">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items.</span></span>
<span data-ttu-id="494c8-186">Para recuperar o deltaLink mais recente, chame `delta` com um parâmetro de cadeia de caracteres de consulta `?token=latest`.</span><span class="sxs-lookup"><span data-stu-id="494c8-186">To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="494c8-187">**Observação: Se você estiver tentando manter uma representação local completa dos itens em uma pasta ou unidade, use `delta` para a enumeração inicial. Outros métodos, como fazer a paginação por meio da coleção `children` de uma pasta, não garantirá o retorno de todos os itens se ocorrerem gravações durante a enumeração. O uso de `delta` é a única maneira de garantir a leitura de todos os dados necessários.**</span><span class="sxs-lookup"><span data-stu-id="494c8-187">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="494c8-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="494c8-188">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="494c8-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="494c8-189">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "files.read", "target": "action" } -->

```msgraph-interactive
GET /me/drive/root/delta?token=latest
```
# <a name="c"></a>[<span data-ttu-id="494c8-190">C#</span><span class="sxs-lookup"><span data-stu-id="494c8-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-latest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="494c8-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="494c8-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-latest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="494c8-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="494c8-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-latest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="494c8-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="494c8-193">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="494c8-194">Comentários</span><span class="sxs-lookup"><span data-stu-id="494c8-194">Remarks</span></span>

* <span data-ttu-id="494c8-p111">O feed delta mostra o estado mais recente de cada item, e não cada alteração. Se um item tiver sido renomeado duas vezes, ele só aparecerá uma vez, com seu nome mais recente.</span><span class="sxs-lookup"><span data-stu-id="494c8-p111">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="494c8-p112">O mesmo item pode aparecer mais de uma vez em um feed delta, por vários motivos. Você deve usar a última ocorrência que visualizar.</span><span class="sxs-lookup"><span data-stu-id="494c8-p112">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="494c8-p113">A propriedade `parentReference` em itens não incluirá um valor para **path**. Isso ocorre porque a renomeação de uma pasta não faz com que os descendentes dessa pasta sejam retornados de **delta**. **Ao usar delta, você sempre deve controlar itens por id**.</span><span class="sxs-lookup"><span data-stu-id="494c8-p113">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="494c8-202">No OneDrive for Business e no SharePoint, `delta` tem suporte apenas na pasta `root`, e não em outras pastas dentro de uma unidade.</span><span class="sxs-lookup"><span data-stu-id="494c8-202">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders within a drive.</span></span>

* <span data-ttu-id="494c8-203">A consulta delta não retornará algumas propriedades DriveItem, dependendo da operação e do tipo de serviço, conforme mostrado nas tabelas a seguir.</span><span class="sxs-lookup"><span data-stu-id="494c8-203">Delta query will not return some DriveItem properties, depending on the operation and service type, as shown in the following tables.</span></span>

    <span data-ttu-id="494c8-204">**OneDrive for Business**</span><span class="sxs-lookup"><span data-stu-id="494c8-204">**OneDrive for Business**</span></span>
    
    | <span data-ttu-id="494c8-205">Tipo de operação</span><span class="sxs-lookup"><span data-stu-id="494c8-205">Operation type</span></span> | <span data-ttu-id="494c8-206">Propriedades omitidas pela consulta delta</span><span class="sxs-lookup"><span data-stu-id="494c8-206">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="494c8-207">Criar/Modificar</span><span class="sxs-lookup"><span data-stu-id="494c8-207">Create/Modify</span></span> | <span data-ttu-id="494c8-208">`ctag`, `lastModifiedBy`</span><span class="sxs-lookup"><span data-stu-id="494c8-208">`ctag`, `lastModifiedBy`</span></span> |
    | <span data-ttu-id="494c8-209">Excluir</span><span class="sxs-lookup"><span data-stu-id="494c8-209">Delete</span></span> | <span data-ttu-id="494c8-210">`ctag`, `lastModifiedBy`, `name`</span><span class="sxs-lookup"><span data-stu-id="494c8-210">`ctag`, `lastModifiedBy`, `name`</span></span> |


    <span data-ttu-id="494c8-211">**OneDrive (consumidor)**</span><span class="sxs-lookup"><span data-stu-id="494c8-211">**OneDrive (consumer)**</span></span>
    
    | <span data-ttu-id="494c8-212">Tipo de operação</span><span class="sxs-lookup"><span data-stu-id="494c8-212">Operation type</span></span> | <span data-ttu-id="494c8-213">Propriedades omitidas pela consulta delta</span><span class="sxs-lookup"><span data-stu-id="494c8-213">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="494c8-214">Criar/Modificar</span><span class="sxs-lookup"><span data-stu-id="494c8-214">Create/Modify</span></span> | <span data-ttu-id="494c8-215">n/d</span><span class="sxs-lookup"><span data-stu-id="494c8-215">n/a</span></span> |
    | <span data-ttu-id="494c8-216">Excluir</span><span class="sxs-lookup"><span data-stu-id="494c8-216">Delete</span></span> | <span data-ttu-id="494c8-217">`ctag`, `size`</span><span class="sxs-lookup"><span data-stu-id="494c8-217">`ctag`, `size`</span></span> |

## <a name="error-responses"></a><span data-ttu-id="494c8-218">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="494c8-218">Error responses</span></span>

<span data-ttu-id="494c8-219">Além dos erros de ressincronização detalhados acima, confira os detalhes sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="494c8-219">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": [
  ]
}
-->
