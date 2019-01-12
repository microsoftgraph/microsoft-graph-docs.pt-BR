---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Sincronizar o conteúdo de uma unidade
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b879b99fb03ab17af4701c96c4be973f1f752be9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991290"
---
# <a name="track-changes-for-a-drive"></a><span data-ttu-id="a2bf2-102">Controlar alterações para uma unidade</span><span class="sxs-lookup"><span data-stu-id="a2bf2-102">Track changes for a Drive</span></span>

> <span data-ttu-id="a2bf2-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2bf2-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2bf2-105">Esse método permite que o seu aplicativo controle alterações em uma unidade e seus filhos com o passar do tempo.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-105">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="a2bf2-p102">Seu aplicativo começa chamando `delta` sem parâmetros. O serviço começa a enumerar a hierarquia da unidade, retornando páginas de itens e um `@odata.nextLink` ou `@odata.deltaLink`, conforme descrito abaixo. Seu aplicativo deve continuar chamando com o `@odata.nextLink` até que você não veja mais um `@odata.nextLink` retornado ou até que você veja uma resposta com um conjunto vazio de alterações.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-p102">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="a2bf2-p103">Quando terminar de receber todas as alterações, você pode aplicá-las ao seu estado local. Para verificar se há alterações no futuro, chame `delta` novamente com o `@odata.deltaLink` da resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-p103">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="a2bf2-p104">Itens excluídos são retornados com a [faceta `deleted`](../resources/deleted.md). Itens com esse conjunto de propriedades devem ser removidos do seu estado local.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-p104">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="a2bf2-113">**Observação:** você apenas deverá excluir uma pasta localmente se ela ficar vazia após a sincronização de todas as alterações.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-113">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2bf2-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2bf2-114">Permissions</span></span>

<span data-ttu-id="a2bf2-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2bf2-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2bf2-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2bf2-117">Permission type</span></span>      | <span data-ttu-id="a2bf2-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2bf2-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2bf2-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2bf2-119">Delegated (work or school account)</span></span> | <span data-ttu-id="a2bf2-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2bf2-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2bf2-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2bf2-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2bf2-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2bf2-122">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a2bf2-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2bf2-123">Application</span></span> | <span data-ttu-id="a2bf2-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2bf2-124">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2bf2-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2bf2-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a><span data-ttu-id="a2bf2-126">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a2bf2-126">Function parameters</span></span>

| <span data-ttu-id="a2bf2-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a2bf2-127">Parameter</span></span>   | <span data-ttu-id="a2bf2-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2bf2-128">Type</span></span>  | <span data-ttu-id="a2bf2-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2bf2-129">Description</span></span>                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a2bf2-130">token</span><span class="sxs-lookup"><span data-stu-id="a2bf2-130">token</span></span>  | <span data-ttu-id="a2bf2-131">string</span><span class="sxs-lookup"><span data-stu-id="a2bf2-131">string</span></span> | <span data-ttu-id="a2bf2-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-132">Optional.</span></span> <span data-ttu-id="a2bf2-133">Se não for especificado, enumera o estado atual da hierarquia.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-133">If unspecified, enumerates the hierarchy's current state.</span></span> <span data-ttu-id="a2bf2-134">Se `latest`, retorna esvaziar a resposta com o token de delta mais recente.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-134">If `latest`, returns empty response with latest delta token.</span></span> <span data-ttu-id="a2bf2-135">Se um token delta anterior, retorna o novo estado desde esse token.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-135">If a previous delta token, returns new state since that token.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="a2bf2-136">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a2bf2-136">Optional query parameters</span></span>

<span data-ttu-id="a2bf2-137">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$select`, `$expand` e `$top` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-137">This method supports the `$select`, `$expand`, and `$top` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="a2bf2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2bf2-138">Response</span></span>

<span data-ttu-id="a2bf2-139">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Driveitem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-139">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="a2bf2-140">Além da coleção de DriveItems, a resposta também incluirá uma das seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="a2bf2-140">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="a2bf2-141">Nome</span><span class="sxs-lookup"><span data-stu-id="a2bf2-141">Name</span></span>                 | <span data-ttu-id="a2bf2-142">Valor</span><span class="sxs-lookup"><span data-stu-id="a2bf2-142">Value</span></span>  | <span data-ttu-id="a2bf2-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2bf2-143">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a2bf2-144">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="a2bf2-144">**@odata.nextLink**</span></span>  | <span data-ttu-id="a2bf2-145">url</span><span class="sxs-lookup"><span data-stu-id="a2bf2-145">url</span></span>    | <span data-ttu-id="a2bf2-146">Uma URL para recuperar a próxima página disponível de alterações, se houver alterações adicionais no conjunto atual.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-146">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="a2bf2-147">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="a2bf2-147">**@odata.deltaLink**</span></span> | <span data-ttu-id="a2bf2-148">url</span><span class="sxs-lookup"><span data-stu-id="a2bf2-148">url</span></span>    | <span data-ttu-id="a2bf2-p107">Uma URL retornada no lugar de **@odata.nextLink** após o retorno de todas as alterações atuais. Usada para ler o próximo conjunto de alterações no futuro.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-p107">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |

## <a name="example-initial-request"></a><span data-ttu-id="a2bf2-151">Exemplo (solicitação inicial)</span><span class="sxs-lookup"><span data-stu-id="a2bf2-151">Example (Initial Request)</span></span>

<span data-ttu-id="a2bf2-152">Veja a seguir um exemplo de como chamar essa API para estabelecer seu estado local.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-152">Here is an example of how to call this API to establish your local state.</span></span>

### <a name="request"></a><span data-ttu-id="a2bf2-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2bf2-153">Request</span></span>

<span data-ttu-id="a2bf2-154">Veja a seguir um exemplo da solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-154">Here is an example of the initial request.</span></span>

<!-- { "blockType": "request", "name": "get_item_delta_first" } -->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

### <a name="response"></a><span data-ttu-id="a2bf2-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2bf2-155">Response</span></span>

<span data-ttu-id="a2bf2-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-156">Here is an example of the response.</span></span>

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

<span data-ttu-id="a2bf2-p108">Essa resposta inclui a primeira página de alterações, e a propriedade **@odata.nextLink** indica que há mais itens disponíveis no conjunto atual de itens. Seu aplicativo deve continuar a solicitar o valor de URL de **@odata.nextLink** até que todas as páginas de itens tenham sido recuperadas.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-p108">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="a2bf2-159">Exemplo (última página de um conjunto)</span><span class="sxs-lookup"><span data-stu-id="a2bf2-159">Example (Last page in a set)</span></span>

<span data-ttu-id="a2bf2-160">Veja a seguir um exemplo de como chamar essa API para atualizar seu estado local.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-160">Here is an example of how to call this API to update your local state.</span></span>

### <a name="request"></a><span data-ttu-id="a2bf2-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2bf2-161">Request</span></span>

<span data-ttu-id="a2bf2-162">Veja a seguir um exemplo da solicitação após a solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-162">Here is an example request after the initial request.</span></span>

<!-- { "blockType": "request", "name": "get_item_delta_last" }-->

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

### <a name="response"></a><span data-ttu-id="a2bf2-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2bf2-163">Response</span></span>

<span data-ttu-id="a2bf2-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-164">Here is an example of the response.</span></span>

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

<span data-ttu-id="a2bf2-165">Essa resposta indica que o item denominado `folder2` foi excluído e que o item `file.txt` foi adicionado ou modificado entre a solicitação inicial e essa solicitação para atualizar o estado local.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-165">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="a2bf2-166">A página final de itens incluirá a propriedade **@odata.deltaLink**, que fornece a URL que poderá ser usada posteriormente para recuperar alterações desde o conjunto atual de itens.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-166">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

<span data-ttu-id="a2bf2-p109">Pode haver casos em que o serviço não pode fornecer uma lista de alterações para um determinado token (por exemplo, se um cliente tentar reutilizar um token antigo depois de ter permanecido desconectado por um longo período, ou se o estado do servidor tiver mudado e um novo token for obrigatório). Nesses casos, o serviço retornará um erro `HTTP 410 Gone` com uma resposta de erro contendo um dos códigos de erro abaixo e um cabeçalho `Location` contendo um novo nextLink que inicia uma enumeração delta do zero. Depois de concluir a enumeração completa, compare os itens retornados com seu estado local e siga estas instruções.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-p109">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="a2bf2-170">Tipo de erro</span><span class="sxs-lookup"><span data-stu-id="a2bf2-170">Error Type</span></span>                       | <span data-ttu-id="a2bf2-171">Instruções</span><span class="sxs-lookup"><span data-stu-id="a2bf2-171">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="a2bf2-p110">Substitua todos os itens locais pela versão do servidor (incluindo exclusões) se você tiver certeza de que o serviço estava atualizado com suas alterações locais quando você sincronizou pela última vez. Carregue alterações locais que o servidor não conhece.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-p110">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="a2bf2-174">Carregue os itens locais que o serviço não retornou e carregue os arquivos que diferem da versão do servidor (mantendo ambas as cópias se você não tiver certeza de qual é a mais atual).</span><span class="sxs-lookup"><span data-stu-id="a2bf2-174">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |

## <a name="retrieving-the-current-deltalink"></a><span data-ttu-id="a2bf2-175">Recuperar o deltaLink atual</span><span class="sxs-lookup"><span data-stu-id="a2bf2-175">Retrieving the current deltaLink</span></span>

<span data-ttu-id="a2bf2-176">Em alguns cenários, pode ser útil solicitar o valor do deltaLink atual sem primeiro enumerar todos os itens que já estão na unidade.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-176">In some scenarios, it may be useful to request the current deltaLink value without first enumerating all of the items in the drive already.</span></span>

<span data-ttu-id="a2bf2-177">Isso poderá ser útil se o seu aplicativo quiser saber apenas sobre as alterações, e não quiser saber sobre os itens existentes.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-177">This can be useful if your app only wants to know about changes, and doesn't need to know about existing items.</span></span>
<span data-ttu-id="a2bf2-178">Para recuperar o deltaLink mais recente, chame `delta` com um parâmetro de cadeia de caracteres de consulta `?token=latest`.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-178">To retrieve the latest deltaLink, call `delta` with a query string parameter `?token=latest`.</span></span>

<span data-ttu-id="a2bf2-179">**Observação: Se você estiver tentando manter uma representação local completa dos itens em uma pasta ou unidade, use `delta` para a enumeração inicial. Outros métodos, como fazer a paginação por meio da coleção `children` de uma pasta, não garantirá o retorno de todos os itens se ocorrerem gravações durante a enumeração. O uso de `delta` é a única maneira de garantir a leitura de todos os dados necessários.**</span><span class="sxs-lookup"><span data-stu-id="a2bf2-179">**Note: If you are trying to maintain a full local representation of the items in a folder or a drive, you must use `delta` for the initial enumeration. Other approaches, such as paging through the `children` collection of a folder, are not guaranteed to return every single item if any writes take place during the enumeration. Using `delta` is the only way to guarantee that you've read all of the data you need to.**</span></span>

### <a name="request"></a><span data-ttu-id="a2bf2-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2bf2-180">Request</span></span>

<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "files.read", "target": "action" } -->

```http
GET /me/drive/root/delta?token=latest
```

### <a name="response"></a><span data-ttu-id="a2bf2-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2bf2-181">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

## <a name="remarks"></a><span data-ttu-id="a2bf2-182">Comentários</span><span class="sxs-lookup"><span data-stu-id="a2bf2-182">Remarks</span></span>

* <span data-ttu-id="a2bf2-p112">O feed delta mostra o estado mais recente de cada item, e não cada alteração. Se um item tiver sido renomeado duas vezes, ele só aparecerá uma vez, com seu nome mais recente.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-p112">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="a2bf2-p113">O mesmo item pode aparecer mais de uma vez em um feed delta, por vários motivos. Você deve usar a última ocorrência que visualizar.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-p113">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="a2bf2-p114">A propriedade `parentReference` em itens não incluirá um valor para **path**. Isso ocorre porque a renomeação de uma pasta não faz com que os descendentes dessa pasta sejam retornados de **delta**. **Ao usar delta, você sempre deve controlar itens por id**.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-p114">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>
* <span data-ttu-id="a2bf2-190">No OneDrive for Business e no SharePoint, `delta` só tem suporte na pasta `root`, e não em outras pastas dentro de uma unidade.</span><span class="sxs-lookup"><span data-stu-id="a2bf2-190">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders within a drive.</span></span>

* <span data-ttu-id="a2bf2-191">O delta não retornará as seguintes propriedades de DriveItem:</span><span class="sxs-lookup"><span data-stu-id="a2bf2-191">Delta will not return the following DriveItem properties:</span></span>

* <span data-ttu-id="a2bf2-192">**cTag**</span><span class="sxs-lookup"><span data-stu-id="a2bf2-192">**cTag**</span></span>
* <span data-ttu-id="a2bf2-193">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="a2bf2-193">**lastModifiedBy**</span></span>
* <span data-ttu-id="a2bf2-194">**size**</span><span class="sxs-lookup"><span data-stu-id="a2bf2-194">**size**</span></span>

## <a name="error-responses"></a><span data-ttu-id="a2bf2-195">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="a2bf2-195">Error responses</span></span>

<span data-ttu-id="a2bf2-196">Além dos erros de ressincronização detalhados acima, confira os detalhes sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="a2bf2-196">In addition to the resync errors detailed above, see [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes"
} -->
