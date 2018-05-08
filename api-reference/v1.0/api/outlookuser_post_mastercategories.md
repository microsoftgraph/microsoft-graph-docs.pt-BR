# <a name="create-outlook-category"></a><span data-ttu-id="04377-101">Criar categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="04377-101">Create Outlook category</span></span>


<span data-ttu-id="04377-102">Cria um objeto [outlookCategory](../resources/outlookCategory.md) na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="04377-102">Create an [outlookCategory](../resources/outlookCategory.md) object in the user's master list of categories.</span></span>

## <a name="permissions"></a><span data-ttu-id="04377-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="04377-103">Permissions</span></span>
<span data-ttu-id="04377-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="04377-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04377-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04377-106">Permission type</span></span>      | <span data-ttu-id="04377-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04377-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04377-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04377-108">Delegated (work or school account)</span></span> | <span data-ttu-id="04377-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04377-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="04377-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04377-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04377-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04377-111">MailboxSettings.ReadWrite</span></span>   |
|<span data-ttu-id="04377-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04377-112">Application</span></span> | <span data-ttu-id="04377-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04377-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="04377-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04377-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/masterCategories
POST /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="request-headers"></a><span data-ttu-id="04377-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04377-115">Request headers</span></span>
| <span data-ttu-id="04377-116">Nome</span><span class="sxs-lookup"><span data-stu-id="04377-116">Name</span></span>       | <span data-ttu-id="04377-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="04377-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="04377-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="04377-118">Authorization</span></span>  | <span data-ttu-id="04377-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04377-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="04377-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04377-121">Request body</span></span>
<span data-ttu-id="04377-122">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookCategory.md).</span><span class="sxs-lookup"><span data-stu-id="04377-122">In the request body, supply a JSON representation of [plannerTask](../resources/outlookCategory.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="04377-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="04377-123">Response</span></span>

<span data-ttu-id="04377-124">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [outlookCategory](../resources/outlookCategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04377-124">If successful, this method returns `201 Created` response code and the new [page](../resources/outlookCategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04377-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04377-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04377-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04377-126">Request</span></span>
<span data-ttu-id="04377-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04377-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlookcategory_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/outlook/masterCategories
Content-type: application/json
Content-Length: 70

{
      "displayName":"Project expenses",
      "color":"preset9"
}
```
<span data-ttu-id="04377-128">No corpo da solicitação, forneça uma representação JSON do objeto [outlookCategory](../resources/outlookCategory.md).</span><span class="sxs-lookup"><span data-stu-id="04377-128">In the request body, supply a JSON representation of [plannerTask](../resources/outlookCategory.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="04377-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="04377-129">Response</span></span>
<span data-ttu-id="04377-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04377-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 250

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->