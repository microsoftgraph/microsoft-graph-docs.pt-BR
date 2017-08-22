# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="a21ae-101">Obtenha uma pasta especial por nome</span><span class="sxs-lookup"><span data-stu-id="a21ae-101">Get a special folder by name</span></span>

<span data-ttu-id="a21ae-102">Use a coleção especial para acessar uma pasta especial pelo nome.</span><span class="sxs-lookup"><span data-stu-id="a21ae-102">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="a21ae-p101">Pastas especiais fornecem aliases simples para acessar pastas conhecidas no OneDrive sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a localizar a pasta.</span><span class="sxs-lookup"><span data-stu-id="a21ae-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="a21ae-p102">As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.</span><span class="sxs-lookup"><span data-stu-id="a21ae-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="a21ae-107">**Observação:**  Se tiver permissões somente leitura e solicitar uma pasta especial que não exista, você receberá um erro `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="a21ae-107">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a21ae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a21ae-108">Prerequisites</span></span>
<span data-ttu-id="a21ae-109">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="a21ae-109">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="a21ae-110">Files.Read</span><span class="sxs-lookup"><span data-stu-id="a21ae-110">Files.Read</span></span>
* <span data-ttu-id="a21ae-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a21ae-111">Files.ReadWrite</span></span>
* <span data-ttu-id="a21ae-112">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="a21ae-112">Files.Read.All</span></span>
* <span data-ttu-id="a21ae-113">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a21ae-113">Files.ReadWrite.All</span></span>
* <span data-ttu-id="a21ae-114">Files.ReadWrite.AppFolder</span><span class="sxs-lookup"><span data-stu-id="a21ae-114">Files.ReadWrite.AppFolder</span></span>
* <span data-ttu-id="a21ae-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="a21ae-115">Sites.Read.All</span></span>
* <span data-ttu-id="a21ae-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a21ae-116">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a21ae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a21ae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/special/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a21ae-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a21ae-118">Optional query parameters</span></span>
<span data-ttu-id="a21ae-119">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a21ae-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a21ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a21ae-120">Request headers</span></span>

| <span data-ttu-id="a21ae-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a21ae-121">Name</span></span>          | <span data-ttu-id="a21ae-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a21ae-122">Type</span></span>   | <span data-ttu-id="a21ae-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a21ae-123">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="a21ae-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a21ae-124">Authorization</span></span> | <span data-ttu-id="a21ae-125">string</span><span class="sxs-lookup"><span data-stu-id="a21ae-125">string</span></span> | <span data-ttu-id="a21ae-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a21ae-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a21ae-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a21ae-128">Request body</span></span>
<span data-ttu-id="a21ae-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a21ae-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a21ae-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a21ae-130">Response</span></span>

<span data-ttu-id="a21ae-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [driveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a21ae-131">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a21ae-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a21ae-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a21ae-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a21ae-133">Request</span></span>
<span data-ttu-id="a21ae-134">Eis um exemplo da solicitação de unidades do usuário.</span><span class="sxs-lookup"><span data-stu-id="a21ae-134">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a><span data-ttu-id="a21ae-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a21ae-135">Response</span></span>
<span data-ttu-id="a21ae-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a21ae-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <a name="remarks"></a><span data-ttu-id="a21ae-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="a21ae-137">Remarks</span></span>

<span data-ttu-id="a21ae-138">Para solicitar os filhos de uma pasta especial, você pode solicitar a coleção `children` ou usar a opção [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para expandir a coleção de filhos.</span><span class="sxs-lookup"><span data-stu-id="a21ae-138">To request the children of a special folder, you can request the `children` collection or use the [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
