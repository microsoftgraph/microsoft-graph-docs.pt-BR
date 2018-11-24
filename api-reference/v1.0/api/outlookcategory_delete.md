# <a name="delete-outlook-category"></a><span data-ttu-id="135ab-101">Excluir categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="135ab-101">Delete Outlook category</span></span>


<span data-ttu-id="135ab-102">Exclua o objeto [outlookCategory](../resources/outlookCategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="135ab-102">Delete the specified [outlookCategory](../resources/outlookCategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="135ab-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="135ab-103">Permissions</span></span>
<span data-ttu-id="135ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="135ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="135ab-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="135ab-106">Permission type</span></span>      | <span data-ttu-id="135ab-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="135ab-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="135ab-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="135ab-108">Delegated (work or school account)</span></span> | <span data-ttu-id="135ab-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="135ab-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="135ab-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="135ab-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="135ab-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="135ab-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="135ab-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="135ab-112">Application</span></span> | <span data-ttu-id="135ab-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="135ab-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="135ab-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="135ab-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="135ab-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="135ab-115">Optional query parameters</span></span>
<span data-ttu-id="135ab-116">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="135ab-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="135ab-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="135ab-117">Request headers</span></span>
| <span data-ttu-id="135ab-118">Nome</span><span class="sxs-lookup"><span data-stu-id="135ab-118">Name</span></span>      |<span data-ttu-id="135ab-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="135ab-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="135ab-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="135ab-120">Authorization</span></span>  | <span data-ttu-id="135ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="135ab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="135ab-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="135ab-123">Request body</span></span>
<span data-ttu-id="135ab-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="135ab-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="135ab-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="135ab-125">Response</span></span>

<span data-ttu-id="135ab-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="135ab-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="135ab-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="135ab-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="135ab-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="135ab-129">Request</span></span>
<span data-ttu-id="135ab-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="135ab-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
##### <a name="response"></a><span data-ttu-id="135ab-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="135ab-131">Response</span></span>
<span data-ttu-id="135ab-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="135ab-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->