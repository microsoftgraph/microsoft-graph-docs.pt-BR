# <a name="update-photo"></a><span data-ttu-id="fb657-101">Atualizar foto</span><span class="sxs-lookup"><span data-stu-id="fb657-101">Update photo</span></span>

<span data-ttu-id="fb657-102">Atualize as propriedades do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="fb657-102">Update the properties of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb657-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb657-103">Permissions</span></span>
<span data-ttu-id="fb657-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb657-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb657-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb657-106">Permission type</span></span>      | <span data-ttu-id="fb657-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb657-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb657-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb657-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fb657-109">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb657-109">Not supported.</span></span>    |
|<span data-ttu-id="fb657-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb657-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb657-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb657-111">Not supported.</span></span>    |
|<span data-ttu-id="fb657-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb657-112">Application</span></span> | <span data-ttu-id="fb657-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb657-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb657-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb657-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="fb657-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-115">Request headers</span></span>
| <span data-ttu-id="fb657-116">Nome</span><span class="sxs-lookup"><span data-stu-id="fb657-116">Name</span></span>       | <span data-ttu-id="fb657-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb657-117">Type</span></span> | <span data-ttu-id="fb657-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb657-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fb657-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb657-119">Authorization</span></span>  | <span data-ttu-id="fb657-120">string</span><span class="sxs-lookup"><span data-stu-id="fb657-120">string</span></span>  | <span data-ttu-id="fb657-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb657-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb657-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-123">Request body</span></span>
<span data-ttu-id="fb657-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="fb657-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fb657-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb657-127">Property</span></span>     | <span data-ttu-id="fb657-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb657-128">Type</span></span>   |<span data-ttu-id="fb657-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb657-129">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="fb657-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-130">Response</span></span>

<span data-ttu-id="fb657-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [photo](../resources/photo.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb657-131">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb657-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb657-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb657-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb657-133">Request</span></span>
<span data-ttu-id="fb657-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb657-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="response"></a><span data-ttu-id="fb657-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb657-135">Response</span></span>
<span data-ttu-id="fb657-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb657-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
