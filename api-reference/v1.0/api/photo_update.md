# <a name="update-photo"></a><span data-ttu-id="b7915-101">Atualizar foto</span><span class="sxs-lookup"><span data-stu-id="b7915-101">Update photo</span></span>

<span data-ttu-id="b7915-102">Atualize as propriedades do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="b7915-102">Update the properties of photo object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b7915-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7915-103">Prerequisites</span></span>
<span data-ttu-id="b7915-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="b7915-104">One of the following **scopes** is required to execute this API:</span></span>
## <a name="http-request"></a><span data-ttu-id="b7915-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7915-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/photo
PATCH /groups/{id}/photo
PATCH /drive/root/createdByUser/photo
```

## <a name="request-headers"></a><span data-ttu-id="b7915-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7915-106">Request headers</span></span>
| <span data-ttu-id="b7915-107">Nome</span><span class="sxs-lookup"><span data-stu-id="b7915-107">Name</span></span>       | <span data-ttu-id="b7915-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7915-108">Type</span></span> | <span data-ttu-id="b7915-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7915-109">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b7915-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7915-110">Authorization</span></span>  | <span data-ttu-id="b7915-111">string</span><span class="sxs-lookup"><span data-stu-id="b7915-111">string</span></span>  | <span data-ttu-id="b7915-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7915-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b7915-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7915-114">Request body</span></span>
<span data-ttu-id="b7915-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b7915-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b7915-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7915-118">Property</span></span>     | <span data-ttu-id="b7915-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7915-119">Type</span></span>   |<span data-ttu-id="b7915-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7915-120">Description</span></span>|
|:---------------|:--------|:----------|

## <a name="response"></a><span data-ttu-id="b7915-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7915-121">Response</span></span>

<span data-ttu-id="b7915-122">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [photo](../resources/photo.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7915-122">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7915-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7915-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7915-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7915-124">Request</span></span>
<span data-ttu-id="b7915-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7915-125">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b7915-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7915-126">Response</span></span>
<span data-ttu-id="b7915-127">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7915-127">Here is an example of the response.</span></span>
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
