# <a name="update-contactfolder"></a><span data-ttu-id="acc5d-101">Atualizar contactfolder</span><span class="sxs-lookup"><span data-stu-id="acc5d-101">Update contactfolder</span></span>

<span data-ttu-id="acc5d-102">Atualiza as propriedades do objeto contactfolder.</span><span class="sxs-lookup"><span data-stu-id="acc5d-102">Update the properties of contactfolder object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="acc5d-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="acc5d-103">Prerequisites</span></span>
<span data-ttu-id="acc5d-104">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="acc5d-104">One of the following **scopes** is required to execute this API: *Contacts.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="acc5d-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acc5d-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="acc5d-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acc5d-106">Request headers</span></span>
| <span data-ttu-id="acc5d-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="acc5d-107">Header</span></span>       | <span data-ttu-id="acc5d-108">Valor</span><span class="sxs-lookup"><span data-stu-id="acc5d-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="acc5d-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="acc5d-109">Authorization</span></span>  | <span data-ttu-id="acc5d-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acc5d-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="acc5d-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="acc5d-112">Content-Type</span></span>  | <span data-ttu-id="acc5d-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acc5d-p102">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="acc5d-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acc5d-115">Request body</span></span>
<span data-ttu-id="acc5d-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="acc5d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="acc5d-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acc5d-119">Property</span></span>     | <span data-ttu-id="acc5d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="acc5d-120">Type</span></span>   |<span data-ttu-id="acc5d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="acc5d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acc5d-122">displayName</span><span class="sxs-lookup"><span data-stu-id="acc5d-122">displayName</span></span>|<span data-ttu-id="acc5d-123">String</span><span class="sxs-lookup"><span data-stu-id="acc5d-123">String</span></span>|<span data-ttu-id="acc5d-124">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="acc5d-124">The folder's display name.</span></span>|
|<span data-ttu-id="acc5d-125">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="acc5d-125">parentFolderId</span></span>|<span data-ttu-id="acc5d-126">String</span><span class="sxs-lookup"><span data-stu-id="acc5d-126">String</span></span>|<span data-ttu-id="acc5d-127">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="acc5d-127">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="acc5d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="acc5d-128">Response</span></span>

<span data-ttu-id="acc5d-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contactFolder](../resources/contactfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="acc5d-129">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="acc5d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="acc5d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acc5d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acc5d-131">Request</span></span>
<span data-ttu-id="acc5d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="acc5d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="acc5d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="acc5d-133">Response</span></span>
<span data-ttu-id="acc5d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="acc5d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
