# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="f51c7-101">Criar um link de compartilhamento para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="f51c7-101">Create a sharing link for a DriveItem</span></span>

<span data-ttu-id="f51c7-102">Você pode usar a ação **createLink** para compartilhar um [DriveItem](../resources/driveitem.md) por meio de um link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="f51c7-102">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="f51c7-p101">A ação **createLink** criará um novo link de compartilhamento se o tipo de link especificado não existir para o aplicativo de chamada. Se um link de compartilhamento do tipo especificado já existir para o aplicativo, o link de compartilhamento existente será retornado.</span><span class="sxs-lookup"><span data-stu-id="f51c7-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="f51c7-105">Recursos de DriveItem herdam permissões de seus ancestrais.</span><span class="sxs-lookup"><span data-stu-id="f51c7-105">DriveItem resources inherit permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="f51c7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f51c7-106">Permissions</span></span>
<span data-ttu-id="f51c7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f51c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f51c7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f51c7-109">Permission type</span></span>      | <span data-ttu-id="f51c7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f51c7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f51c7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f51c7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f51c7-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f51c7-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f51c7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f51c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f51c7-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f51c7-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f51c7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f51c7-115">Application</span></span> | <span data-ttu-id="f51c7-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f51c7-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f51c7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f51c7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/createLink
POST /me/drive/root:/{item-path}:/createLink
POST /groups/{group-id}/drive/items/{item-id}/createLink
POST /drives/{drive-id}/items/{item-id}/createLink
```

## <a name="request-body"></a><span data-ttu-id="f51c7-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f51c7-118">Request body</span></span>
<span data-ttu-id="f51c7-p103">O corpo da solicitação define o tipo de link de compartilhamento que seu aplicativo está procurando. A solicitação deve ser um objeto JSON com essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="f51c7-p103">The body of the request defines the type of sharing link your application is looking for. The request should be a JSON object with this property.</span></span>

| <span data-ttu-id="f51c7-121">Name</span><span class="sxs-lookup"><span data-stu-id="f51c7-121">Name</span></span>      | <span data-ttu-id="f51c7-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f51c7-122">Type</span></span>   | <span data-ttu-id="f51c7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f51c7-123">Description</span></span>                                                                  |
|:----------|:-------|:-----------------------------------------------------------------------------|
| <span data-ttu-id="f51c7-124">**type**</span><span class="sxs-lookup"><span data-stu-id="f51c7-124">**type**</span></span>  | <span data-ttu-id="f51c7-125">string</span><span class="sxs-lookup"><span data-stu-id="f51c7-125">string</span></span> | <span data-ttu-id="f51c7-p104">O tipo de link de compartilhamento a ser criado. Pode ser `view`, `edit` ou `embed`.</span><span class="sxs-lookup"><span data-stu-id="f51c7-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="f51c7-128">**scope**</span><span class="sxs-lookup"><span data-stu-id="f51c7-128">**scope**</span></span> | <span data-ttu-id="f51c7-129">string</span><span class="sxs-lookup"><span data-stu-id="f51c7-129">string</span></span> | <span data-ttu-id="f51c7-p105">O escopo do link a ser criado. Pode ser `anonymous` ou `organization`. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f51c7-p105">The scope of link to create. Either `anonymous` or `organization`. Optional.</span></span> |

## <a name="link-types"></a><span data-ttu-id="f51c7-133">Tipos de link</span><span class="sxs-lookup"><span data-stu-id="f51c7-133">Link types</span></span>
<span data-ttu-id="f51c7-134">Os seguintes valores são permitidos para o parâmetro **type**.</span><span class="sxs-lookup"><span data-stu-id="f51c7-134">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="f51c7-135">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="f51c7-135">Type value</span></span> | <span data-ttu-id="f51c7-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="f51c7-136">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="f51c7-137">Cria um link somente leitura para o item.</span><span class="sxs-lookup"><span data-stu-id="f51c7-137">Creates a read-only link to the item.</span></span>                                                        |
| `edit`     | <span data-ttu-id="f51c7-138">Cria um link de leitura e gravação para o item.</span><span class="sxs-lookup"><span data-stu-id="f51c7-138">Creates a read-write link to the item.</span></span>                                                       |
| `embed`    | <span data-ttu-id="f51c7-p106">Cria um link inserível para o item. Essa opção só está disponível para uso pessoal do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f51c7-p106">Creates an embeddable link to the item. This option is only available for OneDrive Personal.</span></span> |

## <a name="scope-types"></a><span data-ttu-id="f51c7-141">Tipos de escopo</span><span class="sxs-lookup"><span data-stu-id="f51c7-141">Scope types</span></span>
<span data-ttu-id="f51c7-p107">Os seguintes valores são permitidos para o parâmetro **scope**. Esse é um parâmetro opcional. Se o parâmetro **scope** não for especificado, o link mais permissivo disponível será criado.</span><span class="sxs-lookup"><span data-stu-id="f51c7-p107">The following values are allowed for the **scope** parameter. This is an optional parameter. If the **scope** parameter is not specified, the most permissive link available will be created.</span></span>

| <span data-ttu-id="f51c7-145">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="f51c7-145">Type value</span></span>     | <span data-ttu-id="f51c7-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="f51c7-146">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="f51c7-p108">Cria um link para o item que pode ser acessado por qualquer pessoa. Links anônimos podem estar desabilitados pelo administrador de locatários.</span><span class="sxs-lookup"><span data-stu-id="f51c7-p108">Creates a link to the item accessible to anyone. Anonymous links may be disabled by the tenant administrator.</span></span>                 |
| `organization` | <span data-ttu-id="f51c7-p109">Cria um link para o item que pode ser acessado dentro de uma organização. O escopo de link de organização não está disponível para uso pessoal do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f51c7-p109">Creates a link to the item accessible within an organization. Organization link scope is not available for OneDrive Personal.</span></span> |

## <a name="response"></a><span data-ttu-id="f51c7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f51c7-151">Response</span></span>

<span data-ttu-id="f51c7-152">Se for bem-sucedido, esse método retornará um único recurso [Permission](../resources/permission.md) no corpo da resposta, que representa a permissão solicitada do link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="f51c7-152">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing link permission.</span></span>

<span data-ttu-id="f51c7-153">O serviço primeiro examinará as permissões atuais e verificará se já existe uma permissão com o mesmo valor de **type** para o aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="f51c7-153">The service will first look at the current permissions and check if one already exists that has the same **type** for the calling application.</span></span>

<span data-ttu-id="f51c7-154">A resposta será `201 Created` se um novo link de compartilhamento for criado para o item ou `200 OK` se um link existente for retornado.</span><span class="sxs-lookup"><span data-stu-id="f51c7-154">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="f51c7-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f51c7-155">Example</span></span>
<span data-ttu-id="f51c7-156">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f51c7-156">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f51c7-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f51c7-157">Request</span></span>
<span data-ttu-id="f51c7-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f51c7-158">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

##### <a name="response"></a><span data-ttu-id="f51c7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f51c7-159">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a><span data-ttu-id="f51c7-160">Criando links compartilháveis pela empresa</span><span class="sxs-lookup"><span data-stu-id="f51c7-160">Creating company sharable links</span></span>

<span data-ttu-id="f51c7-p110">O OneDrive for Business e o SharePoint oferecem suporte a links compartilháveis pela empresa. Estes são semelhantes a links anônimos, com a diferença de que apenas funcionam para membros do locatário proprietário. Para criar um link compartilhável pela empresa, use o parâmetro **scope** com um valor de `organization`.</span><span class="sxs-lookup"><span data-stu-id="f51c7-p110">OneDrive for Business and SharePoint support company sharable links. These are similar to anonymous links, except they only work for members of the owning tenant. To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

## <a name="http-request"></a><span data-ttu-id="f51c7-164">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f51c7-164">HTTP request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->
```
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

## <a name="http-response"></a><span data-ttu-id="f51c7-165">Resposta HTTP</span><span class="sxs-lookup"><span data-stu-id="f51c7-165">HTTP response</span></span>

<span data-ttu-id="f51c7-166">A resposta será `201 Created` se um novo link de compartilhamento for criado para o item ou `200 OK` se um link existente for retornado.</span><span class="sxs-lookup"><span data-stu-id="f51c7-166">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="embeddable-links"></a><span data-ttu-id="f51c7-167">Links inseríveis</span><span class="sxs-lookup"><span data-stu-id="f51c7-167">Embeddable links</span></span>

<span data-ttu-id="f51c7-p111">Ao usar o tipo de link `embed`, a webUrl retornada pode ser inserida em um elemento HTML `<iframe>`. Quando um link de inserção é criado, a propriedade `webHtml` contém o código HTML de um `<iframe>` para hospedar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f51c7-p111">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="f51c7-170">**Observação:** Links de inserção apenas têm suporte em [Drives](../resources/drive.md), em que **driveType** é `personal`.</span><span class="sxs-lookup"><span data-stu-id="f51c7-170">**Note:** Embed links are only supported in [Drives](../resources/drive.md) where the **driveType** is `personal`.</span></span>

## <a name="remarks"></a><span data-ttu-id="f51c7-171">Comentários</span><span class="sxs-lookup"><span data-stu-id="f51c7-171">Remarks</span></span>

* <span data-ttu-id="f51c7-172">Links criados usando esta ação não expiram, a menos que uma política de expiração padrão seja imposta à organização.</span><span class="sxs-lookup"><span data-stu-id="f51c7-172">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="f51c7-173">Os links ficam visíveis nas permissões de compartilhamento do item e podem ser removidos por um proprietário desse item.</span><span class="sxs-lookup"><span data-stu-id="f51c7-173">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="f51c7-174">Os links sempre apontam para a versão atual de um item, a menos que esse item esteja em check-out (apenas no SharePoint).</span><span class="sxs-lookup"><span data-stu-id="f51c7-174">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: createLink",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Create sharing link"
} -->
