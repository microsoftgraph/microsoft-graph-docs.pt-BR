# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="e91ff-101">Obtenha uma pasta especial por nome</span><span class="sxs-lookup"><span data-stu-id="e91ff-101">Get a special folder by name</span></span>

<span data-ttu-id="e91ff-102">Use a coleção especial para acessar uma pasta especial pelo nome.</span><span class="sxs-lookup"><span data-stu-id="e91ff-102">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="e91ff-p101">Pastas especiais fornecem aliases simples para acessar pastas conhecidas no OneDrive sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a localizar a pasta.</span><span class="sxs-lookup"><span data-stu-id="e91ff-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="e91ff-p102">As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.</span><span class="sxs-lookup"><span data-stu-id="e91ff-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

><span data-ttu-id="e91ff-107">**Observação:**  Se tiver permissões somente leitura e solicitar uma pasta especial que não exista, você receberá um erro `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="e91ff-107">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="e91ff-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e91ff-108">Permissions</span></span>

<span data-ttu-id="e91ff-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e91ff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e91ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e91ff-111">Permission type</span></span>                        | <span data-ttu-id="e91ff-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e91ff-112">Permissions (from least to most privileged)</span></span>                                                           |
|:--------------------------------------|:------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e91ff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e91ff-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e91ff-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e91ff-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="e91ff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e91ff-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e91ff-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Files.ReadWrite.AppFolder</span><span class="sxs-lookup"><span data-stu-id="e91ff-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Files.ReadWrite.AppFolder</span></span>           |
|<span data-ttu-id="e91ff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e91ff-117">Application</span></span>                            | <span data-ttu-id="e91ff-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e91ff-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="e91ff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e91ff-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/special/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e91ff-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e91ff-120">Optional query parameters</span></span>

<span data-ttu-id="e91ff-121">Este método oferece suporte aos [parâmetros de consulta OData](../../../concepts/query_parameters.md) `$expand` e `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e91ff-121">This method supports the `$expand` and `$select` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e91ff-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e91ff-122">Request headers</span></span>

| <span data-ttu-id="e91ff-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e91ff-123">Name</span></span>          | <span data-ttu-id="e91ff-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e91ff-124">Type</span></span>   | <span data-ttu-id="e91ff-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e91ff-125">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="e91ff-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e91ff-126">Authorization</span></span> | <span data-ttu-id="e91ff-127">string</span><span class="sxs-lookup"><span data-stu-id="e91ff-127">string</span></span> | <span data-ttu-id="e91ff-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e91ff-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e91ff-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e91ff-130">Request body</span></span>

<span data-ttu-id="e91ff-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e91ff-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e91ff-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e91ff-132">Response</span></span>

<span data-ttu-id="e91ff-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [driveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e91ff-133">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e91ff-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e91ff-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e91ff-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e91ff-135">Request</span></span>

<span data-ttu-id="e91ff-136">Eis um exemplo da solicitação de unidades do usuário.</span><span class="sxs-lookup"><span data-stu-id="e91ff-136">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a><span data-ttu-id="e91ff-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e91ff-137">Response</span></span>
<span data-ttu-id="e91ff-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e91ff-138">Here is an example of the response.</span></span>
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

## <a name="remarks"></a><span data-ttu-id="e91ff-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="e91ff-139">Remarks</span></span>

<span data-ttu-id="e91ff-140">Para solicitar os filhos de uma pasta especial, você pode solicitar a coleção `children` ou usar a opção [$expand](../../../concepts/query_parameters.md) para expandir a coleção de filhos.</span><span class="sxs-lookup"><span data-stu-id="e91ff-140">To request the children of a special folder, you can request the `children` collection or use the [expand](../../../concepts/query_parameters.md) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
