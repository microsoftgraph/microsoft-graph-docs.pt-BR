# <a name="update-contactfolder"></a><span data-ttu-id="1931f-101">Atualizar contactfolder</span><span class="sxs-lookup"><span data-stu-id="1931f-101">Update contactfolder</span></span>

<span data-ttu-id="1931f-102">Atualizar as propriedades do objeto contactfolder.</span><span class="sxs-lookup"><span data-stu-id="1931f-102">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1931f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="1931f-103">Permissions</span></span>
<span data-ttu-id="1931f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1931f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1931f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1931f-106">Permission type</span></span>      | <span data-ttu-id="1931f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1931f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1931f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1931f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1931f-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1931f-109">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1931f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1931f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1931f-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1931f-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1931f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1931f-112">Application</span></span> | <span data-ttu-id="1931f-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1931f-113">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1931f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1931f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1931f-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1931f-115">Request headers</span></span>
| <span data-ttu-id="1931f-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1931f-116">Header</span></span>       | <span data-ttu-id="1931f-117">Valor</span><span class="sxs-lookup"><span data-stu-id="1931f-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1931f-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="1931f-118">Authorization</span></span>  | <span data-ttu-id="1931f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1931f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1931f-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1931f-121">Content-Type</span></span>  | <span data-ttu-id="1931f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1931f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1931f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1931f-124">Request body</span></span>
<span data-ttu-id="1931f-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1931f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1931f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1931f-128">Property</span></span>     | <span data-ttu-id="1931f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1931f-129">Type</span></span>   |<span data-ttu-id="1931f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1931f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1931f-131">displayName</span><span class="sxs-lookup"><span data-stu-id="1931f-131">displayName</span></span>|<span data-ttu-id="1931f-132">String</span><span class="sxs-lookup"><span data-stu-id="1931f-132">String</span></span>|<span data-ttu-id="1931f-133">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="1931f-133">The folder's display name.</span></span>|
|<span data-ttu-id="1931f-134">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="1931f-134">parentFolderId</span></span>|<span data-ttu-id="1931f-135">String</span><span class="sxs-lookup"><span data-stu-id="1931f-135">String</span></span>|<span data-ttu-id="1931f-136">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="1931f-136">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="1931f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1931f-137">Response</span></span>

<span data-ttu-id="1931f-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contactFolder](../resources/contactfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1931f-138">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1931f-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1931f-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1931f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1931f-140">Request</span></span>
<span data-ttu-id="1931f-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1931f-141">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="1931f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1931f-142">Response</span></span>
<span data-ttu-id="1931f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1931f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
