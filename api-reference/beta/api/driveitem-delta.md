---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Sincronizar o conteúdo de uma unidade
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ad99a7dd701c52def0879a8611cc49f96e4654b3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325255"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="d97ed-102">Controlar alterações para uma unidade</span><span class="sxs-lookup"><span data-stu-id="d97ed-102">Track changes for a Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d97ed-103">Esse método permite que o seu aplicativo controle alterações em uma unidade e seus filhos com o passar do tempo.</span><span class="sxs-lookup"><span data-stu-id="d97ed-103">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="d97ed-p101">Seu aplicativo começa chamando `delta` sem parâmetros. O serviço começa a enumerar a hierarquia da unidade, retornando páginas de itens e um `@odata.nextLink` ou `@odata.deltaLink`, conforme descrito abaixo. Seu aplicativo deve continuar chamando com o `@odata.nextLink` até que você não veja mais um `@odata.nextLink` retornado ou até que você veja uma resposta com um conjunto vazio de alterações.</span><span class="sxs-lookup"><span data-stu-id="d97ed-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="d97ed-p102">Quando terminar de receber todas as alterações, você pode aplicá-las ao seu estado local. Para verificar se há alterações no futuro, chame `delta` novamente com o `@odata.deltaLink` da resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="d97ed-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="d97ed-p103">Itens excluídos são retornados com a [faceta `deleted`](../resources/deleted.md). Itens com esse conjunto de propriedades devem ser removidos do seu estado local.</span><span class="sxs-lookup"><span data-stu-id="d97ed-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="d97ed-111">**Observação:** você apenas deverá excluir uma pasta localmente se ela ficar vazia após a sincronização de todas as alterações.</span><span class="sxs-lookup"><span data-stu-id="d97ed-111">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="d97ed-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="d97ed-112">Permissions</span></span>

<span data-ttu-id="d97ed-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d97ed-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d97ed-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d97ed-115">Permission type</span></span>      | <span data-ttu-id="d97ed-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d97ed-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d97ed-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d97ed-117">Delegated (work or school account)</span></span> | <span data-ttu-id="d97ed-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d97ed-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d97ed-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d97ed-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d97ed-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d97ed-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d97ed-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d97ed-121">Application</span></span> | <span data-ttu-id="d97ed-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d97ed-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d97ed-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d97ed-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="d97ed-124">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d97ed-124">Function parameters</span></span>

| <span data-ttu-id="d97ed-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d97ed-125">Parameter</span></span>   | <span data-ttu-id="d97ed-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d97ed-126">Type</span></span>  | <span data-ttu-id="d97ed-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d97ed-127">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d97ed-128">token</span><span class="sxs-lookup"><span data-stu-id="d97ed-128">token</span></span>  | <span data-ttu-id="d97ed-129">string</span><span class="sxs-lookup"><span data-stu-id="d97ed-129">string</span></span> | <span data-ttu-id="d97ed-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d97ed-130">Optional.</span></span> <span data-ttu-id="d97ed-131">Quando não é especificado, enumera o estado da hierarquia atual.</span><span class="sxs-lookup"><span data-stu-id="d97ed-131">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="d97ed-132">Quando é `latest`, retorna uma resposta vazia com o token delta mais recente.</span><span class="sxs-lookup"><span data-stu-id="d97ed-132">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="d97ed-133">Quando é um token delta anterior, retorna o novo estado após o token.</span><span class="sxs-lookup"><span data-stu-id="d97ed-133">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d97ed-134">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d97ed-134">Optional query parameters</span></span>

<span data-ttu-id="d97ed-135">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$select`, `$expand` e `$top` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="d97ed-135">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="d97ed-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d97ed-136">Response</span></span>

<span data-ttu-id="d97ed-137">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Driveitem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d97ed-137">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="d97ed-138">Além da coleção de DriveItems, a resposta também incluirá uma das seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="d97ed-138">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="d97ed-139">Nome</span><span class="sxs-lookup"><span data-stu-id="d97ed-139">Name</span></span>                 | <span data-ttu-id="d97ed-140">Valor</span><span class="sxs-lookup"><span data-stu-id="d97ed-140">Value</span></span>  | <span data-ttu-id="d97ed-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="d97ed-141">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d97ed-142">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="d97ed-142">**@odata.nextLink**</span></span>  | <span data-ttu-id="d97ed-143">url</span><span class="sxs-lookup"><span data-stu-id="d97ed-143">url</span></span>    | <span data-ttu-id="d97ed-144">Uma URL para recuperar a próxima página disponível de alterações, se houver alterações adicionais no conjunto atual.</span><span class="sxs-lookup"><span data-stu-id="d97ed-144">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="d97ed-145">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="d97ed-145">**@odata.deltaLink**</span></span> | <span data-ttu-id="d97ed-146">url</span><span class="sxs-lookup"><span data-stu-id="d97ed-146">url</span></span>    | <span data-ttu-id="d97ed-p106">Uma URL retornada no lugar de **@odata.nextLink** após o retorno de todas as alterações atuais. Usada para ler o próximo conjunto de alterações no futuro.</span><span class="sxs-lookup"><span data-stu-id="d97ed-p106">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="d97ed-149">Exemplo (solicitação inicial)</span><span class="sxs-lookup"><span data-stu-id="d97ed-149">Example (Initial Request)</span></span>

<span data-ttu-id="d97ed-150">Veja a seguir um exemplo de como chamar essa API para estabelecer seu estado local.</span><span class="sxs-lookup"><span data-stu-id="d97ed-150">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="d97ed-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d97ed-151">Request</span></span>

<span data-ttu-id="d97ed-152">Veja a seguir um exemplo da solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="d97ed-152">Here is an example of the initial request.</span></span>

<!-- { "blockType": "request", "name": "get_item_delta_first" } -->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

### <a name="response"></a><span data-ttu-id="d97ed-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d97ed-153">Response</span></span>

<span data-ttu-id="d97ed-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d97ed-154">Here is an example of the response.</span></span>

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

<span data-ttu-id="d97ed-p107">Essa resposta inclui a primeira página de alterações, e a propriedade **@odata.nextLink** indica que há mais itens disponíveis no conjunto atual de itens. Seu aplicativo deve continuar a solicitar o valor de URL de **@odata.nextLink** até que todas as páginas de itens tenham sido recuperadas.</span><span class="sxs-lookup"><span data-stu-id="d97ed-p107">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="d97ed-157">Exemplo (última página de um conjunto)</span><span class="sxs-lookup"><span data-stu-id="d97ed-157">Example (Last page in a set)</span></span>

<span data-ttu-id="d97ed-158">Veja a seguir um exemplo de como chamar essa API para atualizar seu estado local.</span><span class="sxs-lookup"><span data-stu-id="d97ed-158">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="d97ed-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d97ed-159">Request</span></span>

<span data-ttu-id="d97ed-160">Veja a seguir um exemplo da solicitação após a solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="d97ed-160">Here is an example request after the initial request.</span></span>

<!-- { "blockType": "request", "name": "get_item_delta_last" }-->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

### <a name="response"></a><span data-ttu-id="d97ed-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="d97ed-161">Response</span></span>

<span data-ttu-id="d97ed-162">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d97ed-162">Here is an example of the response.</span></span>

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

<span data-ttu-id="d97ed-163">Essa resposta indica que o item denominado `folder2` foi excluído e que o item `file.txt` foi adicionado ou modificado entre a solicitação inicial e essa solicitação para atualizar o estado local.</span><span class="sxs-lookup"><span data-stu-id="d97ed-163">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="d97ed-164">A página final de itens incluirá a propriedade **@odata.deltaLink**, que fornece a URL que poderá ser usada posteriormente para recuperar alterações desde o conjunto atual de itens.</span><span class="sxs-lookup"><span data-stu-id="d97ed-164">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="d97ed-p108">Pode haver casos em que o serviço não pode fornecer uma lista de alterações para um determinado token (por exemplo, se um cliente tentar reutilizar um token antigo depois de ter permanecido desconectado por um longo período, ou se o estado do servidor tiver mudado e um novo token for obrigatório). Nesses casos, o serviço retornará um erro `HTTP 410 Gone` com uma resposta de erro contendo um dos códigos de erro abaixo e um cabeçalho `Location` contendo um novo nextLink que inicia uma enumeração delta do zero. Depois de concluir a enumeração completa, compare os itens retornados com seu estado local e siga estas instruções.</span><span class="sxs-lookup"><span data-stu-id="d97ed-p108">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="d97ed-168">Tipo de erro</span><span class="sxs-lookup"><span data-stu-id="d97ed-168">Error Type</span></span>                       | <span data-ttu-id="d97ed-169">Instruções</span><span class="sxs-lookup"><span data-stu-id="d97ed-169">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="d97ed-p109">Substitua todos os itens locais pela versão do servidor (incluindo exclusões) se você tiver certeza de que o serviço estava atualizado com suas alterações locais quando você sincronizou pela última vez. Carregue alterações locais que o servidor não conhece.</span><span class="sxs-lookup"><span data-stu-id="d97ed-p109">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="d97ed-172">Carregue os itens locais que o serviço não retornou e carregue os arquivos que diferem da versão do servidor (mantendo ambas as cópias se você não tiver certeza de qual é a mais atual).</span><span class="sxs-lookup"><span data-stu-id="d97ed-172">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="d97ed-173">Recuperar o deltaLink atual</span><span class="sxs-lookup"><span data-stu-id="d97ed-173">Retrieving the current deltaLink</span></span>

<span data-ttu-id="d97ed-174">Em alguns cenários, pode ser útil solicitar o valor do deltaLink atual sem primeiro enumerar todos os itens que já estão na unidade.</span><span class="sxs-lookup"><span data-stu-id="d97ed-174">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="d97ed-175">Isso poderá ser útil se o seu aplicativo quiser saber apenas sobre as alterações, e não quiser saber sobre os itens existentes.</span><span class="sxs-lookup"><span data-stu-id="d97ed-175">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items.</span></span>
<span data-ttu-id="d97ed-176">Para recuperar o deltaLink mais recente, chame `delta` com um parâmetro de cadeia de caracteres de consulta `?token=latest`.</span><span class="sxs-lookup"><span data-stu-id="d97ed-176">To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="d97ed-177">**Observação: Se você estiver tentando manter uma representação local completa dos itens em uma pasta ou unidade, use `delta` para a enumeração inicial. Outros métodos, como fazer a paginação por meio da coleção `children` de uma pasta, não garantirá o retorno de todos os itens se ocorrerem gravações durante a enumeração. O uso de `delta` é a única maneira de garantir a leitura de todos os dados necessários.**</span><span class="sxs-lookup"><span data-stu-id="d97ed-177">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="d97ed-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d97ed-178">Request</span></span>

<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "files.read", "target": "action" } -->

```http
GET /me/drive/root/delta?token=latest
```

### <a name="response"></a><span data-ttu-id="d97ed-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="d97ed-179">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="d97ed-180">Comentários</span><span class="sxs-lookup"><span data-stu-id="d97ed-180">Remarks</span></span>

* <span data-ttu-id="d97ed-p111">O feed delta mostra o estado mais recente de cada item, e não cada alteração. Se um item tiver sido renomeado duas vezes, ele só aparecerá uma vez, com seu nome mais recente.</span><span class="sxs-lookup"><span data-stu-id="d97ed-p111">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="d97ed-p112">O mesmo item pode aparecer mais de uma vez em um feed delta, por vários motivos. Você deve usar a última ocorrência que visualizar.</span><span class="sxs-lookup"><span data-stu-id="d97ed-p112">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="d97ed-p113">A propriedade `parentReference` em itens não incluirá um valor para **path**. Isso ocorre porque a renomeação de uma pasta não faz com que os descendentes dessa pasta sejam retornados de **delta**. **Ao usar delta, você sempre deve controlar itens por id**.</span><span class="sxs-lookup"><span data-stu-id="d97ed-p113">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="d97ed-188">No OneDrive for Business e no SharePoint, `delta` tem suporte apenas na pasta `root`, e não em outras pastas dentro de uma unidade.</span><span class="sxs-lookup"><span data-stu-id="d97ed-188">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders within a drive.</span></span>

* <span data-ttu-id="d97ed-189">A consulta delta não retornará algumas propriedades DriveItem, dependendo da operação e do tipo de serviço, conforme mostrado nas tabelas a seguir.</span><span class="sxs-lookup"><span data-stu-id="d97ed-189">Delta query will not return some DriveItem properties, depending on the operation and service type, as shown in the following tables.</span></span>

    <span data-ttu-id="d97ed-190">**OneDrive for Business**</span><span class="sxs-lookup"><span data-stu-id="d97ed-190">**OneDrive for Business**</span></span>
    
    | <span data-ttu-id="d97ed-191">Tipo de operação</span><span class="sxs-lookup"><span data-stu-id="d97ed-191">Operation type</span></span> | <span data-ttu-id="d97ed-192">Propriedades omitidas pela consulta delta</span><span class="sxs-lookup"><span data-stu-id="d97ed-192">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="d97ed-193">Criar/Modificar</span><span class="sxs-lookup"><span data-stu-id="d97ed-193">Create/Modify</span></span> | <span data-ttu-id="d97ed-194">`ctag`, `lastModifiedBy`</span><span class="sxs-lookup"><span data-stu-id="d97ed-194">`ctag`, `lastModifiedBy`</span></span> |
    | <span data-ttu-id="d97ed-195">Excluir</span><span class="sxs-lookup"><span data-stu-id="d97ed-195">Delete</span></span> | <span data-ttu-id="d97ed-196">`ctag`, `lastModifiedBy`, `name`</span><span class="sxs-lookup"><span data-stu-id="d97ed-196">`ctag`, `lastModifiedBy`, `name`</span></span> |


    <span data-ttu-id="d97ed-197">**OneDrive (consumidor)**</span><span class="sxs-lookup"><span data-stu-id="d97ed-197">**OneDrive (consumer)**</span></span>
    
    | <span data-ttu-id="d97ed-198">Tipo de operação</span><span class="sxs-lookup"><span data-stu-id="d97ed-198">Operation type</span></span> | <span data-ttu-id="d97ed-199">Propriedades omitidas pela consulta delta</span><span class="sxs-lookup"><span data-stu-id="d97ed-199">Properties omitted by delta query</span></span> |
    |---------|----------|
    | <span data-ttu-id="d97ed-200">Criar/Modificar</span><span class="sxs-lookup"><span data-stu-id="d97ed-200">Create/Modify</span></span> | <span data-ttu-id="d97ed-201">n/d</span><span class="sxs-lookup"><span data-stu-id="d97ed-201">n/a</span></span> |
    | <span data-ttu-id="d97ed-202">Excluir</span><span class="sxs-lookup"><span data-stu-id="d97ed-202">Delete</span></span> | <span data-ttu-id="d97ed-203">`ctag`, `size`</span><span class="sxs-lookup"><span data-stu-id="d97ed-203">`ctag`, `size`</span></span> |

## <a name="error-responses"></a><span data-ttu-id="d97ed-204">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="d97ed-204">Error responses</span></span>

<span data-ttu-id="d97ed-205">Além dos erros de ressincronização detalhados acima, confira os detalhes sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="d97ed-205">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": []
}
-->
