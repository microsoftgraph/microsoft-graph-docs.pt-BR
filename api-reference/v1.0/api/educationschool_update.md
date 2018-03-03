# <a name="update-educationschool-properties"></a><span data-ttu-id="9c116-101">Atualizar as propriedades educationschool</span><span class="sxs-lookup"><span data-stu-id="9c116-101">Update educationschool properties</span></span>

<span data-ttu-id="9c116-102">Atualize as propriedades de um objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="9c116-102">Update the properties of a contact object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c116-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c116-103">Permissions</span></span>
<span data-ttu-id="9c116-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9c116-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9c116-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c116-106">Permission type</span></span>      | <span data-ttu-id="9c116-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c116-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c116-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c116-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="9c116-109">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c116-109">Not supported.</span></span>  |
|<span data-ttu-id="9c116-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c116-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9c116-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c116-111">Not supported.</span></span>  |
|<span data-ttu-id="9c116-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c116-112">Application</span></span> | <span data-ttu-id="9c116-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c116-113">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c116-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c116-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9c116-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c116-115">Request headers</span></span>
| <span data-ttu-id="9c116-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c116-116">Header</span></span>       | <span data-ttu-id="9c116-117">Valor</span><span class="sxs-lookup"><span data-stu-id="9c116-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c116-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c116-118">Authorization</span></span>  | <span data-ttu-id="9c116-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c116-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9c116-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c116-121">Content-Type</span></span>  | <span data-ttu-id="9c116-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9c116-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c116-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c116-123">Request body</span></span>
<span data-ttu-id="9c116-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="9c116-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9c116-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9c116-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9c116-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9c116-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9c116-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c116-127">Property</span></span>     | <span data-ttu-id="9c116-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c116-128">Type</span></span>   |<span data-ttu-id="9c116-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c116-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c116-130">displayName</span><span class="sxs-lookup"><span data-stu-id="9c116-130">displayName</span></span>| <span data-ttu-id="9c116-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c116-131">String</span></span>| <span data-ttu-id="9c116-132">Nome de exibição da escola</span><span class="sxs-lookup"><span data-stu-id="9c116-132">Display name of the template.</span></span>| 
|<span data-ttu-id="9c116-133">description</span><span class="sxs-lookup"><span data-stu-id="9c116-133">description</span></span>| <span data-ttu-id="9c116-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c116-134">String</span></span> | <span data-ttu-id="9c116-135">Descrição da escola</span><span class="sxs-lookup"><span data-stu-id="9c116-135">Description of the template.</span></span>| 
|<span data-ttu-id="9c116-136">principalEmail</span><span class="sxs-lookup"><span data-stu-id="9c116-136">principalEmail</span></span>| <span data-ttu-id="9c116-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c116-137">String</span></span>| <span data-ttu-id="9c116-138">Endereço de email da entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="9c116-138">Email address of the principal</span></span>|
|<span data-ttu-id="9c116-139">principalName</span><span class="sxs-lookup"><span data-stu-id="9c116-139">principalName</span></span>| <span data-ttu-id="9c116-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c116-140">String</span></span> | <span data-ttu-id="9c116-141">Nome da entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="9c116-141">Name of the principal</span></span>|
|<span data-ttu-id="9c116-142">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="9c116-142">externalPrincipalId</span></span>| <span data-ttu-id="9c116-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c116-143">String</span></span> | <span data-ttu-id="9c116-144">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="9c116-144">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="9c116-145">highestGrade</span><span class="sxs-lookup"><span data-stu-id="9c116-145">highestGrade</span></span>|<span data-ttu-id="9c116-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c116-146">String</span></span>| <span data-ttu-id="9c116-147">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="9c116-147">Highest grade taught.</span></span> |
|<span data-ttu-id="9c116-148">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="9c116-148">lowestGrade</span></span>|<span data-ttu-id="9c116-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c116-149">String</span></span>| <span data-ttu-id="9c116-150">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="9c116-150">Lowest grade taught.</span></span> |
|<span data-ttu-id="9c116-151">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="9c116-151">schoolNumber</span></span>|<span data-ttu-id="9c116-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c116-152">String</span></span>| <span data-ttu-id="9c116-153">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="9c116-153">School Number.</span></span>|
|<span data-ttu-id="9c116-154">externalId</span><span class="sxs-lookup"><span data-stu-id="9c116-154">externalId</span></span>|<span data-ttu-id="9c116-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c116-155">String</span></span>| <span data-ttu-id="9c116-156">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="9c116-156">Id of school in syncing system.</span></span> |
|<span data-ttu-id="9c116-157">phone</span><span class="sxs-lookup"><span data-stu-id="9c116-157">Phone</span></span>|<span data-ttu-id="9c116-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c116-158">String</span></span>| <span data-ttu-id="9c116-159">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="9c116-159">Phone number of school.</span></span> |
|<span data-ttu-id="9c116-160">fax</span><span class="sxs-lookup"><span data-stu-id="9c116-160">Fax.</span></span>|<span data-ttu-id="9c116-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c116-161">String</span></span>| <span data-ttu-id="9c116-162">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="9c116-162">Fax number of school.</span></span> |
|<span data-ttu-id="9c116-163">address</span><span class="sxs-lookup"><span data-stu-id="9c116-163">address</span></span>|[<span data-ttu-id="9c116-164">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="9c116-164">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="9c116-165">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="9c116-165">Address of the School.</span></span>|
|<span data-ttu-id="9c116-166">createdBy</span><span class="sxs-lookup"><span data-stu-id="9c116-166">createdBy</span></span>|[<span data-ttu-id="9c116-167">identitySet</span><span class="sxs-lookup"><span data-stu-id="9c116-167">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="9c116-168">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="9c116-168">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="9c116-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c116-169">Response</span></span>
<span data-ttu-id="9c116-170">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c116-170">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c116-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c116-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c116-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c116-172">Request</span></span>
<span data-ttu-id="9c116-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c116-173">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/10002
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
##### <a name="response"></a><span data-ttu-id="9c116-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c116-174">Response</span></span>
<span data-ttu-id="9c116-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c116-175">The following is an example of the response.</span></span> 

><span data-ttu-id="9c116-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c116-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
