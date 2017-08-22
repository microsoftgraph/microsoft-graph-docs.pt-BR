# <a name="update-mailfolder"></a><span data-ttu-id="607d9-101">Atualizar mailfolder</span><span class="sxs-lookup"><span data-stu-id="607d9-101">Update mailfolder</span></span>

<span data-ttu-id="607d9-102">Atualize as propriedades do objeto mailfolder.</span><span class="sxs-lookup"><span data-stu-id="607d9-102">Update the properties of mailfolder object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="607d9-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="607d9-103">Prerequisites</span></span>
<span data-ttu-id="607d9-104">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="607d9-104">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="607d9-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="607d9-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="607d9-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="607d9-106">Request headers</span></span>
| <span data-ttu-id="607d9-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="607d9-107">Header</span></span>       | <span data-ttu-id="607d9-108">Valor</span><span class="sxs-lookup"><span data-stu-id="607d9-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="607d9-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="607d9-109">Authorization</span></span>  | <span data-ttu-id="607d9-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="607d9-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="607d9-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="607d9-112">Content-Type</span></span>  | <span data-ttu-id="607d9-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="607d9-p102">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="607d9-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="607d9-115">Request body</span></span>
<span data-ttu-id="607d9-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="607d9-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="607d9-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="607d9-119">Property</span></span>     | <span data-ttu-id="607d9-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="607d9-120">Type</span></span>   |<span data-ttu-id="607d9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="607d9-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="607d9-122">displayName</span><span class="sxs-lookup"><span data-stu-id="607d9-122">displayName</span></span>|<span data-ttu-id="607d9-123">String</span><span class="sxs-lookup"><span data-stu-id="607d9-123">String</span></span>|<span data-ttu-id="607d9-124">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="607d9-124">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="607d9-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="607d9-125">Response</span></span>

<span data-ttu-id="607d9-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="607d9-126">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="607d9-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="607d9-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="607d9-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="607d9-128">Request</span></span>
<span data-ttu-id="607d9-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="607d9-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/{id}
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
##### <a name="response"></a><span data-ttu-id="607d9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="607d9-130">Response</span></span>
<span data-ttu-id="607d9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="607d9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
