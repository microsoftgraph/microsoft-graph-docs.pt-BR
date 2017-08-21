# <a name="track-changes-for-a-drive"></a><span data-ttu-id="18aaa-101">Controlar alterações para uma unidade</span><span class="sxs-lookup"><span data-stu-id="18aaa-101">Track changes for a Drive</span></span>

<span data-ttu-id="18aaa-102">Esse método permite que o seu aplicativo controle alterações em uma unidade e seus filhos com o passar do tempo.</span><span class="sxs-lookup"><span data-stu-id="18aaa-102">This method allows your app to track changes to a drive and its children over time.</span></span>

<span data-ttu-id="18aaa-p101">Seu aplicativo começa chamando `delta` sem parâmetros. O serviço começa a enumerar a hierarquia da unidade, retornando páginas de itens e um `@odata.nextLink` ou `@odata.deltaLink`, conforme descrito abaixo. Seu aplicativo deve continuar chamando com o `@odata.nextLink` até que você não veja mais um `@odata.nextLink` retornado ou até que você veja uma resposta com um conjunto vazio de alterações.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p101">Your app begins by calling `delta` without any parameters. The service starts enumerating the drive's hierarchy, returning pages of items and either an `@odata.nextLink` or an `@odata.deltaLink`, as described below. Your app should continue calling with the `@odata.nextLink` until you no longer see an `@odata.nextLink` returned, or you see a response with an empty set of changes.</span></span>

<span data-ttu-id="18aaa-p102">Quando terminar de receber todas as alterações, você pode aplicá-las ao seu estado local. Para verificar se há alterações no futuro, chame `delta` novamente com o `@odata.deltaLink` da resposta anterior.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p102">After you have finished receiving all the changes, you may apply them to your local state. To check for changes in the future, call `delta` again with the `@odata.deltaLink` from the previous response.</span></span>

<span data-ttu-id="18aaa-p103">Itens excluídos são retornados com a [faceta `deleted`](../resources/deleted.md). Itens com esse conjunto de propriedades devem ser removidos do seu estado local.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p103">Deleted items are returned with the [`deleted` facet](../resources/deleted.md). Items with this property set should be removed from your local state.</span></span> 

<span data-ttu-id="18aaa-110">**Observação:** você apenas deverá excluir uma pasta localmente se ela ficar vazia após a sincronização de todas as alterações.</span><span class="sxs-lookup"><span data-stu-id="18aaa-110">**Note:** you should only delete a folder locally if it is empty after syncing all the changes.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18aaa-111">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18aaa-111">Prerequisites</span></span>
<span data-ttu-id="18aaa-112">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="18aaa-112">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="18aaa-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="18aaa-113">Files.Read</span></span>
* <span data-ttu-id="18aaa-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18aaa-114">Files.ReadWrite</span></span>
* <span data-ttu-id="18aaa-115">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="18aaa-115">Files.Read.All</span></span>
* <span data-ttu-id="18aaa-116">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18aaa-116">Files.ReadWrite.All</span></span>
* <span data-ttu-id="18aaa-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="18aaa-117">Sites.Read.All</span></span>
* <span data-ttu-id="18aaa-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18aaa-118">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="18aaa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18aaa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/delta
GET /drives/{drive-id}/root/delta
GET /groups/{group-id}/drive/root/delta
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18aaa-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="18aaa-120">Optional query parameters</span></span>
<span data-ttu-id="18aaa-121">Este método oferece suporte aos [parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) `$select`, `$expand` e `$top` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="18aaa-121">This method supports `$select`, `$expand`, and `$top` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="18aaa-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18aaa-122">Request body</span></span>
<span data-ttu-id="18aaa-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18aaa-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18aaa-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="18aaa-124">Response</span></span>

<span data-ttu-id="18aaa-125">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Driveitem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18aaa-125">If successful, this method returns a `200 OK` response code and a collection of [DriveItem](../resources/driveitem.md) resources in the response body.</span></span>

<span data-ttu-id="18aaa-126">Além da coleção de DriveItems, a resposta também incluirá uma das seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="18aaa-126">In addition to the collection of DriveItems, the response will also include one of the following properties:</span></span>

| <span data-ttu-id="18aaa-127">Nome</span><span class="sxs-lookup"><span data-stu-id="18aaa-127">Name</span></span>                 | <span data-ttu-id="18aaa-128">Valor</span><span class="sxs-lookup"><span data-stu-id="18aaa-128">Value</span></span>  | <span data-ttu-id="18aaa-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="18aaa-129">Description</span></span>                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="18aaa-130">**@odata.nextLink**</span><span class="sxs-lookup"><span data-stu-id="18aaa-130">**@odata.nextLink**</span></span>  | <span data-ttu-id="18aaa-131">url</span><span class="sxs-lookup"><span data-stu-id="18aaa-131">url</span></span>    | <span data-ttu-id="18aaa-132">Uma URL para recuperar a próxima página disponível de alterações, se houver alterações adicionais no conjunto atual.</span><span class="sxs-lookup"><span data-stu-id="18aaa-132">A URL to retrieve the next available page of changes, if there are additional changes in the current set.</span></span>                                        |
| <span data-ttu-id="18aaa-133">**@odata.deltaLink**</span><span class="sxs-lookup"><span data-stu-id="18aaa-133">**@odata.deltaLink**</span></span> | <span data-ttu-id="18aaa-134">url</span><span class="sxs-lookup"><span data-stu-id="18aaa-134">url</span></span>    | <span data-ttu-id="18aaa-p104">Uma URL retornada no lugar de **@odata.nextLink** após o retorno de todas as alterações atuais. Usada para ler o próximo conjunto de alterações no futuro.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p104">A URL returned instead of **@odata.nextLink** after all current changes have been returned. Used to read the next set of changes in the future.</span></span>  |


## <a name="example-initial-request"></a><span data-ttu-id="18aaa-137">Exemplo (solicitação inicial)</span><span class="sxs-lookup"><span data-stu-id="18aaa-137">Example (Initial Request)</span></span>
<span data-ttu-id="18aaa-138">Veja a seguir um exemplo de como chamar essa API para estabelecer seu estado local.</span><span class="sxs-lookup"><span data-stu-id="18aaa-138">Here is an example of how to call this API to establish your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="18aaa-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18aaa-139">Request</span></span>
<span data-ttu-id="18aaa-140">Veja a seguir um exemplo da solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="18aaa-140">Here is an example of the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta
```

##### <a name="response"></a><span data-ttu-id="18aaa-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="18aaa-141">Response</span></span>
<span data-ttu-id="18aaa-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18aaa-142">Here is an example of the response.</span></span>

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

<span data-ttu-id="18aaa-p105">Essa resposta inclui a primeira página de alterações, e a propriedade **@odata.nextLink** indica que há mais itens disponíveis no conjunto atual de itens. Seu aplicativo deve continuar a solicitar o valor de URL de **@odata.nextLink** até que todas as páginas de itens tenham sido recuperadas.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p105">This response includes the first page of changes, and the **@odata.nextLink** property indicates that there are more items available in the current set of items. Your app should continue to request the URL value of **@odata.nextLink** until all pages of items have been retrieved.</span></span>

## <a name="example-last-page-in-a-set"></a><span data-ttu-id="18aaa-145">Exemplo (última página de um conjunto)</span><span class="sxs-lookup"><span data-stu-id="18aaa-145">Example (Last page in a set)</span></span>
<span data-ttu-id="18aaa-146">Veja a seguir um exemplo de como chamar essa API para atualizar seu estado local.</span><span class="sxs-lookup"><span data-stu-id="18aaa-146">Here is an example of how to call this API to update your local state.</span></span>

##### <a name="request"></a><span data-ttu-id="18aaa-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18aaa-147">Request</span></span>
<span data-ttu-id="18aaa-148">Veja a seguir um exemplo da solicitação após a solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="18aaa-148">Here is an example request after the initial request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/delta(token='1230919asd190410jlka')
```

##### <a name="response"></a><span data-ttu-id="18aaa-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="18aaa-149">Response</span></span>
<span data-ttu-id="18aaa-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18aaa-150">Here is an example of the response.</span></span>

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

<span data-ttu-id="18aaa-151">Essa resposta indica que o item denominado `folder2` foi excluído e que o item `file.txt` foi adicionado ou modificado entre a solicitação inicial e essa solicitação para atualizar o estado local.</span><span class="sxs-lookup"><span data-stu-id="18aaa-151">This response indicates that the item named `folder2` was deleted and the item `file.txt` was either added or modified between the initial request and this request to update the local state.</span></span>

<span data-ttu-id="18aaa-152">A página final de itens incluirá a propriedade **@odata.deltaLink**, que fornece a URL que poderá ser usada posteriormente para recuperar alterações desde o conjunto atual de itens.</span><span class="sxs-lookup"><span data-stu-id="18aaa-152">The final page of items will include the **@odata.deltaLink** property, which provides the URL that can be used later to retrieve changes since the current set of items.</span></span>

## <a name="remarks"></a><span data-ttu-id="18aaa-153">Comentários</span><span class="sxs-lookup"><span data-stu-id="18aaa-153">Remarks</span></span>

* <span data-ttu-id="18aaa-p106">O feed delta mostra o estado mais recente de cada item, e não cada alteração. Se um item tiver sido renomeado duas vezes, ele só aparecerá uma vez, com seu nome mais recente.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p106">The delta feed shows the latest state for each item, not each change. If an item were renamed twice, it would only show up once, with its latest name.</span></span>
* <span data-ttu-id="18aaa-p107">O mesmo item pode aparecer mais de uma vez em um feed delta, por vários motivos. Você deve usar a última ocorrência que visualizar.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p107">The same item may appear more than once in a delta feed, for various reasons. You should use the last occurrence you see.</span></span>
* <span data-ttu-id="18aaa-p108">A propriedade `parentReference` em itens não incluirá um valor para **path**. Isso ocorre porque a renomeação de uma pasta não faz com que os descendentes dessa pasta sejam retornados de **delta**. **Ao usar delta, você sempre deve controlar itens por id**.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p108">The `parentReference` property on items will not include a value for **path**. This occurs because renaming a folder does not result in any descendants of the folder being returned from **delta**. **When using delta you should always track items by id**.</span></span>

<span data-ttu-id="18aaa-p109">Pode haver casos em que o serviço não pode fornecer uma lista de alterações para um determinado token (por exemplo, se um cliente tentar reutilizar um token antigo depois de ter permanecido desconectado por um longo período, ou se o estado do servidor tiver mudado e um novo token for obrigatório). Nesses casos, o serviço retornará um erro `HTTP 410 Gone` com uma resposta de erro contendo um dos códigos de erro abaixo e um cabeçalho `Location` contendo um novo nextLink que inicia uma enumeração delta do zero. Depois de concluir a enumeração completa, compare os itens retornados com seu estado local e siga estas instruções.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p109">There may be cases when the service can't provide a list of changes for a given token (for example, if a client tries to reuse an old token after being disconnected for a long time, or if server state has changed and a new token is required). In these cases the service will return an `HTTP 410 Gone` error with an error response containing one of the error codes below, and a `Location` header containing a new nextLink that starts a fresh delta enumeration from scratch. After finishing the full enumeration, compare the returned items with your local state and follow these instructions.</span></span>

| <span data-ttu-id="18aaa-164">Tipo de erro</span><span class="sxs-lookup"><span data-stu-id="18aaa-164">Error Type</span></span>                       | <span data-ttu-id="18aaa-165">Instruções</span><span class="sxs-lookup"><span data-stu-id="18aaa-165">Instructions</span></span>                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | <span data-ttu-id="18aaa-p110">Substitua todos os itens locais pela versão do servidor (incluindo exclusões) se você tiver certeza de que o serviço estava atualizado com suas alterações locais quando você sincronizou pela última vez. Carregue alterações locais que o servidor não conhece.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p110">Replace any local items with the server's version (including deletes) if you're sure that the service was up to date with your local changes when you last sync'd. Upload any local changes that the server doesn't know about.</span></span> |
| `resyncChangesUploadDifferences` | <span data-ttu-id="18aaa-168">Carregue os itens locais que o serviço não retornou e carregue os arquivos que diferem da versão do servidor (mantendo ambas as cópias se você não tiver certeza de qual é a mais atual).</span><span class="sxs-lookup"><span data-stu-id="18aaa-168">Upload any local items that the service did not return, and upload any files that differ from the server's version (keeping both copies if you're not sure which one is more up-to-date).</span></span>                                       |


<span data-ttu-id="18aaa-p111">No OneDrive for Business e no SharePoint, `delta` só tem suporte na pasta `root`, e não em outras pastas. Ele também não retornará as seguintes propriedades de DriveItem:</span><span class="sxs-lookup"><span data-stu-id="18aaa-p111">In OneDrive for Business and SharePoint, `delta` is only supported on the `root` folder, not on other folders. It also will not return the following DriveItem properties:</span></span>

* <span data-ttu-id="18aaa-171">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="18aaa-171">**createdBy**</span></span>
* <span data-ttu-id="18aaa-172">**cTag**</span><span class="sxs-lookup"><span data-stu-id="18aaa-172">**cTag**</span></span>
* <span data-ttu-id="18aaa-173">**eTag**</span><span class="sxs-lookup"><span data-stu-id="18aaa-173">**etag**</span></span>
* <span data-ttu-id="18aaa-174">**fileSystemInfo**</span><span class="sxs-lookup"><span data-stu-id="18aaa-174">**fileSystemInfo**</span></span>
* <span data-ttu-id="18aaa-175">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="18aaa-175">**lastModifiedBy**</span></span>
* <span data-ttu-id="18aaa-176">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="18aaa-176">**parentReference**</span></span>
* <span data-ttu-id="18aaa-177">**size**</span><span class="sxs-lookup"><span data-stu-id="18aaa-177">**size**</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "Get item delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
