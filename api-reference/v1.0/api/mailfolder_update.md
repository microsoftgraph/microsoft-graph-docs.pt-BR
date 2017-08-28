# <a name="update-mailfolder"></a><span data-ttu-id="31c2d-101">Atualizar mailfolder</span><span class="sxs-lookup"><span data-stu-id="31c2d-101">Update mailfolder</span></span>

<span data-ttu-id="31c2d-102">Atualizar as propriedades do objeto de mailfolder.</span><span class="sxs-lookup"><span data-stu-id="31c2d-102">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="31c2d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="31c2d-103">Permissions</span></span>
<span data-ttu-id="31c2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="31c2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="31c2d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31c2d-106">Permission type</span></span>      | <span data-ttu-id="31c2d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31c2d-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="31c2d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31c2d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="31c2d-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31c2d-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="31c2d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31c2d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31c2d-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31c2d-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="31c2d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31c2d-112">Application</span></span> | <span data-ttu-id="31c2d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31c2d-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="31c2d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31c2d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="31c2d-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31c2d-115">Request headers</span></span>
| <span data-ttu-id="31c2d-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31c2d-116">Header</span></span>       | <span data-ttu-id="31c2d-117">Valor</span><span class="sxs-lookup"><span data-stu-id="31c2d-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31c2d-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="31c2d-118">Authorization</span></span>  | <span data-ttu-id="31c2d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31c2d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="31c2d-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31c2d-121">Content-Type</span></span>  | <span data-ttu-id="31c2d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31c2d-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="31c2d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31c2d-124">Request body</span></span>
<span data-ttu-id="31c2d-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="31c2d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="31c2d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31c2d-128">Property</span></span>     | <span data-ttu-id="31c2d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="31c2d-129">Type</span></span>   |<span data-ttu-id="31c2d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="31c2d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31c2d-131">displayName</span><span class="sxs-lookup"><span data-stu-id="31c2d-131">displayName</span></span>|<span data-ttu-id="31c2d-132">String</span><span class="sxs-lookup"><span data-stu-id="31c2d-132">String</span></span>|<span data-ttu-id="31c2d-133">O nome de exibição da mailFolder.</span><span class="sxs-lookup"><span data-stu-id="31c2d-133">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="31c2d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="31c2d-134">Response</span></span>

<span data-ttu-id="31c2d-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31c2d-135">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31c2d-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31c2d-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31c2d-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31c2d-137">Request</span></span>
<span data-ttu-id="31c2d-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31c2d-138">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="31c2d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="31c2d-139">Response</span></span>
<span data-ttu-id="31c2d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31c2d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
