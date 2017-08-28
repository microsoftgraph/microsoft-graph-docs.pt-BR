# <a name="track-changes-for-a-drive"></a><span data-ttu-id="86697-101">Controlar alterações para uma unidade</span><span class="sxs-lookup"><span data-stu-id="86697-101">Track changes for a Drive</span></span>

<span data-ttu-id="86697-102">Esse método permite que o seu aplicativo controle alterações em uma unidade e seus filhos com o passar do tempo.</span><span class="sxs-lookup"><span data-stu-id="86697-102">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="86697-p101">Seu aplicativo começa chamando `delta` sem parâmetros. O serviço começa a enumerar a hierarquia da unidade, retornando páginas de itens e um `@odata.nextLink` ou `@odata.deltaLink`, conforme descrito abaixo. Seu aplicativo deve continuar chamando com o `@odata.nextLink` até que você não veja mais um `@odata.nextLink` retornado ou até que você veja uma resposta com um conjunto vazio de alterações.</span><span class="sxs-lookup"><span data-stu-id="86697-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="86697-p102">Quando terminar de receber todas as alterações, você pode aplicá-las ao seu estado local. Para verificar se há alterações no futuro, chame `delta` novamente com o `@odata.deltaLink` da resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="86697-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="86697-p103">Itens excluídos são retornados com a [faceta `deleted`](../resources/deleted.md). Itens com esse conjunto de propriedades devem ser removidos do seu estado local.</span><span class="sxs-lookup"><span data-stu-id="86697-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="86697-110">**Observação:** você apenas deverá excluir uma pasta localmente se ela ficar vazia após a sincronização de todas as alterações.</span><span class="sxs-lookup"><span data-stu-id="86697-110">Note: you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="86697-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="86697-111">Permissions</span></span>
<span data-ttu-id="86697-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="86697-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="86697-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86697-114">Permission type</span></span>      | <span data-ttu-id="86697-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86697-115">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="86697-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86697-116">Delegated (work or school account)</span></span> | <span data-ttu-id="86697-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86697-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="86697-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86697-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86697-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86697-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="86697-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86697-120">Application</span></span> | <span data-ttu-id="86697-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86697-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="86697-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86697-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/delta
GET /drives/{drive-id}/root/delta
GET /groups/{group-id}/drive/root/delta
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86697-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="86697-123">Optional query parameters</span></span>
<span data-ttu-id="86697-124">Este método oferece suporte aos [parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) `$select`, `$expand` e `$top` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="86697-124">This method supports `$select`, `$expand`, and `$top` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="86697-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86697-125">Request body</span></span>
<span data-ttu-id="86697-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="86697-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86697-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="86697-127">Response</span></span>

<span data-ttu-id="86697-128">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Driveitem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86697-128">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="86697-129">Além da coleção de DriveItems, a resposta também incluirá uma das seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="86697-129">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="86697-130">Nome</span><span class="sxs-lookup"><span data-stu-id="86697-130">Name</span></span>                 | <span data-ttu-id="86697-131">Valor</span><span class="sxs-lookup"><span data-stu-id="86697-131">Value</span></span>  | <span data-ttu-id="86697-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="86697-132">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="86697-133">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="86697-133">**@odata.nextLink**</span></span>  | <span data-ttu-id="86697-134">url</span><span class="sxs-lookup"><span data-stu-id="86697-134">url</span></span>    | <span data-ttu-id="86697-135">Uma URL para recuperar a próxima página disponível de alterações, se houver alterações adicionais no conjunto atual.</span><span class="sxs-lookup"><span data-stu-id="86697-135">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="86697-136">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="86697-136">**@odata.deltaLink**</span></span> | <span data-ttu-id="86697-137">url</span><span class="sxs-lookup"><span data-stu-id="86697-137">url</span></span>    | <span data-ttu-id="86697-p105">Uma URL retornada no lugar de **@odata.nextLink** após o retorno de todas as alterações atuais. Usada para ler o próximo conjunto de alterações no futuro.</span><span class="sxs-lookup"><span data-stu-id="86697-p105">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |


## <a name="example-initial-request"></a><span data-ttu-id="86697-140">Exemplo (solicitação inicial)</span><span class="sxs-lookup"><span data-stu-id="86697-140">Example (Initial Request)</span></span>
<span data-ttu-id="86697-141">Veja a seguir um exemplo de como chamar essa API para estabelecer seu estado local.</span><span class="sxs-lookup"><span data-stu-id="86697-141">Here is an example of how to call this API to establish your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="86697-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86697-142">Request</span></span>
<span data-ttu-id="86697-143">Veja a seguir um exemplo da solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="86697-143">Here is an example of the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

##### <a name="response"></a><span data-ttu-id="86697-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="86697-144">Response</span></span>
<span data-ttu-id="86697-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86697-145">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
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

<span data-ttu-id="86697-p106">Essa resposta inclui a primeira página de alterações, e a propriedade **@odata.nextLink** indica que há mais itens disponíveis no conjunto atual de itens. Seu aplicativo deve continuar a solicitar o valor de URL de **@odata.nextLink** até que todas as páginas de itens tenham sido recuperadas.</span><span class="sxs-lookup"><span data-stu-id="86697-p106">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="86697-148">Exemplo (última página de um conjunto)</span><span class="sxs-lookup"><span data-stu-id="86697-148">Example (Last page in a set)</span></span>
<span data-ttu-id="86697-149">Veja a seguir um exemplo de como chamar essa API para atualizar seu estado local.</span><span class="sxs-lookup"><span data-stu-id="86697-149">Here is an example of how to call this API to update your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="86697-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86697-150">Request</span></span>
<span data-ttu-id="86697-151">Veja a seguir um exemplo da solicitação após a solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="86697-151">Here is an example request after the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

##### <a name="response"></a><span data-ttu-id="86697-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="86697-152">Response</span></span>
<span data-ttu-id="86697-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86697-153">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
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

<span data-ttu-id="86697-154">Essa resposta indica que o item denominado `folder2` foi excluído e que o item `file.txt` foi adicionado ou modificado entre a solicitação inicial e essa solicitação para atualizar o estado local.</span><span class="sxs-lookup"><span data-stu-id="86697-154">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="86697-155">A página final de itens incluirá a propriedade **@odata.deltaLink**, que fornece a URL que poderá ser usada posteriormente para recuperar alterações desde o conjunto atual de itens.</span><span class="sxs-lookup"><span data-stu-id="86697-155">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

## <a name="remarks"></a><span data-ttu-id="86697-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="86697-156">Remarks</span></span>

* <span data-ttu-id="86697-p107">O feed delta mostra o estado mais recente de cada item, e não cada alteração. Se um item tiver sido renomeado duas vezes, ele só aparecerá uma vez, com seu nome mais recente.</span><span class="sxs-lookup"><span data-stu-id="86697-p107">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="86697-p108">O mesmo item pode aparecer mais de uma vez em um feed delta, por vários motivos. Você deve usar a última ocorrência que visualizar.</span><span class="sxs-lookup"><span data-stu-id="86697-p108">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="86697-p109">A propriedade `parentReference` em itens não incluirá um valor para **path**. Isso ocorre porque a renomeação de uma pasta não faz com que os descendentes dessa pasta sejam retornados de **delta**. **Ao usar delta, você sempre deve controlar itens por id**.</span><span class="sxs-lookup"><span data-stu-id="86697-p109">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>

<span data-ttu-id="86697-p110">Pode haver casos em que o serviço não pode fornecer uma lista de alterações para um determinado token (por exemplo, se um cliente tentar reutilizar um token antigo depois de ter permanecido desconectado por um longo período, ou se o estado do servidor tiver mudado e um novo token for obrigatório). Nesses casos, o serviço retornará um erro `HTTP 410 Gone` com uma resposta de erro contendo um dos códigos de erro abaixo e um cabeçalho `Location` contendo um novo nextLink que inicia uma enumeração delta do zero. Depois de concluir a enumeração completa, compare os itens retornados com seu estado local e siga estas instruções.</span><span class="sxs-lookup"><span data-stu-id="86697-p110">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="86697-167">Tipo de erro</span><span class="sxs-lookup"><span data-stu-id="86697-167">Error Type</span></span>                       | <span data-ttu-id="86697-168">Instruções</span><span class="sxs-lookup"><span data-stu-id="86697-168">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="86697-p111">Substitua todos os itens locais pela versão do servidor (incluindo exclusões) se você tiver certeza de que o serviço estava atualizado com suas alterações locais quando você sincronizou pela última vez. Carregue alterações locais que o servidor não conhece.</span><span class="sxs-lookup"><span data-stu-id="86697-p111">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="86697-171">Carregue os itens locais que o serviço não retornou e carregue os arquivos que diferem da versão do servidor (mantendo ambas as cópias se você não tiver certeza de qual é a mais atual).</span><span class="sxs-lookup"><span data-stu-id="86697-171">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |


<span data-ttu-id="86697-p112">No OneDrive for Business e no SharePoint, `delta` só tem suporte na pasta `root`, e não em outras pastas. Ele também não retornará as seguintes propriedades de DriveItem:</span><span class="sxs-lookup"><span data-stu-id="86697-p112">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders. It also will not return the following DriveItem properties:</span></span>

* <span data-ttu-id="86697-174">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="86697-174">**createdBy**</span></span>
* <span data-ttu-id="86697-175">**cTag**</span><span class="sxs-lookup"><span data-stu-id="86697-175">**cTag**</span></span>
* <span data-ttu-id="86697-176">**eTag**</span><span class="sxs-lookup"><span data-stu-id="86697-176">**etag**</span></span>
* <span data-ttu-id="86697-177">**fileSystemInfo**</span><span class="sxs-lookup"><span data-stu-id="86697-177">**fileSystemInfo**</span></span>
* <span data-ttu-id="86697-178">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="86697-178">**lastModifiedBy**</span></span>
* <span data-ttu-id="86697-179">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="86697-179">**parentReference**</span></span>
* <span data-ttu-id="86697-180">**size**</span><span class="sxs-lookup"><span data-stu-id="86697-180">**size**</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "Get item delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
