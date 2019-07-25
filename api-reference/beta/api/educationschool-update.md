---
title: Atualizar as propriedades educationschool
description: Atualize as propriedades de um objeto de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7688e57b38ff6788425a217e76afdec146944a22
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860182"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="980ab-103">Atualizar as propriedades educationschool</span><span class="sxs-lookup"><span data-stu-id="980ab-103">Update educationschool properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="980ab-104">Atualize as propriedades de um objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="980ab-104">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="980ab-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="980ab-105">Permissions</span></span>
<span data-ttu-id="980ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="980ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="980ab-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="980ab-108">Permission type</span></span>      | <span data-ttu-id="980ab-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="980ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="980ab-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="980ab-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="980ab-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="980ab-111">Not supported.</span></span>  |
|<span data-ttu-id="980ab-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="980ab-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="980ab-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="980ab-113">Not supported.</span></span>  |
|<span data-ttu-id="980ab-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="980ab-114">Application</span></span> | <span data-ttu-id="980ab-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="980ab-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="980ab-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="980ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="980ab-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="980ab-117">Request headers</span></span>
| <span data-ttu-id="980ab-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="980ab-118">Header</span></span>       | <span data-ttu-id="980ab-119">Valor</span><span class="sxs-lookup"><span data-stu-id="980ab-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="980ab-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="980ab-120">Authorization</span></span>  | <span data-ttu-id="980ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="980ab-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="980ab-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="980ab-123">Content-Type</span></span>  | <span data-ttu-id="980ab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="980ab-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="980ab-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="980ab-125">Request body</span></span>
<span data-ttu-id="980ab-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="980ab-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="980ab-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="980ab-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="980ab-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="980ab-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="980ab-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="980ab-129">Property</span></span>     | <span data-ttu-id="980ab-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="980ab-130">Type</span></span>   |<span data-ttu-id="980ab-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="980ab-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="980ab-132">displayName</span><span class="sxs-lookup"><span data-stu-id="980ab-132">displayName</span></span>| <span data-ttu-id="980ab-133">String</span><span class="sxs-lookup"><span data-stu-id="980ab-133">String</span></span>| <span data-ttu-id="980ab-134">Nome de exibição da escola</span><span class="sxs-lookup"><span data-stu-id="980ab-134">Display name of the school</span></span>| 
|<span data-ttu-id="980ab-135">descrição</span><span class="sxs-lookup"><span data-stu-id="980ab-135">description</span></span>| <span data-ttu-id="980ab-136">String</span><span class="sxs-lookup"><span data-stu-id="980ab-136">String</span></span> | <span data-ttu-id="980ab-137">Descrição da escola</span><span class="sxs-lookup"><span data-stu-id="980ab-137">Description of the school</span></span>| 
|<span data-ttu-id="980ab-138">principalEmail</span><span class="sxs-lookup"><span data-stu-id="980ab-138">principalEmail</span></span>| <span data-ttu-id="980ab-139">String</span><span class="sxs-lookup"><span data-stu-id="980ab-139">String</span></span>| <span data-ttu-id="980ab-140">Endereço de email da entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="980ab-140">Email address of the principal</span></span>|
|<span data-ttu-id="980ab-141">principalName</span><span class="sxs-lookup"><span data-stu-id="980ab-141">principalName</span></span>| <span data-ttu-id="980ab-142">String</span><span class="sxs-lookup"><span data-stu-id="980ab-142">String</span></span> | <span data-ttu-id="980ab-143">Nome da entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="980ab-143">Name of the principal</span></span>|
|<span data-ttu-id="980ab-144">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="980ab-144">externalPrincipalId</span></span>| <span data-ttu-id="980ab-145">String</span><span class="sxs-lookup"><span data-stu-id="980ab-145">String</span></span> | <span data-ttu-id="980ab-146">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="980ab-146">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="980ab-147">highestGrade</span><span class="sxs-lookup"><span data-stu-id="980ab-147">highestGrade</span></span>|<span data-ttu-id="980ab-148">String</span><span class="sxs-lookup"><span data-stu-id="980ab-148">String</span></span>| <span data-ttu-id="980ab-149">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="980ab-149">Highest grade taught.</span></span> |
|<span data-ttu-id="980ab-150">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="980ab-150">lowestGrade</span></span>|<span data-ttu-id="980ab-151">String</span><span class="sxs-lookup"><span data-stu-id="980ab-151">String</span></span>| <span data-ttu-id="980ab-152">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="980ab-152">Lowest grade taught.</span></span> |
|<span data-ttu-id="980ab-153">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="980ab-153">schoolNumber</span></span>|<span data-ttu-id="980ab-154">String</span><span class="sxs-lookup"><span data-stu-id="980ab-154">String</span></span>| <span data-ttu-id="980ab-155">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="980ab-155">School Number.</span></span>|
|<span data-ttu-id="980ab-156">externalId</span><span class="sxs-lookup"><span data-stu-id="980ab-156">externalId</span></span>|<span data-ttu-id="980ab-157">String</span><span class="sxs-lookup"><span data-stu-id="980ab-157">String</span></span>| <span data-ttu-id="980ab-158">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="980ab-158">Id of school in syncing system.</span></span> |
|<span data-ttu-id="980ab-159">phone</span><span class="sxs-lookup"><span data-stu-id="980ab-159">phone</span></span>|<span data-ttu-id="980ab-160">String</span><span class="sxs-lookup"><span data-stu-id="980ab-160">String</span></span>| <span data-ttu-id="980ab-161">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="980ab-161">Phone number of school.</span></span> |
|<span data-ttu-id="980ab-162">fax</span><span class="sxs-lookup"><span data-stu-id="980ab-162">fax</span></span>|<span data-ttu-id="980ab-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="980ab-163">String</span></span>| <span data-ttu-id="980ab-164">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="980ab-164">Fax number of school.</span></span> |
|<span data-ttu-id="980ab-165">address</span><span class="sxs-lookup"><span data-stu-id="980ab-165">address</span></span>|[<span data-ttu-id="980ab-166">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="980ab-166">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="980ab-167">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="980ab-167">Address of the School.</span></span>|
|<span data-ttu-id="980ab-168">createdBy</span><span class="sxs-lookup"><span data-stu-id="980ab-168">createdBy</span></span>|[<span data-ttu-id="980ab-169">identitySet</span><span class="sxs-lookup"><span data-stu-id="980ab-169">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="980ab-170">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="980ab-170">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="980ab-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="980ab-171">Response</span></span>
<span data-ttu-id="980ab-172">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="980ab-172">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="980ab-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="980ab-173">Example</span></span>
##### <a name="request"></a><span data-ttu-id="980ab-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="980ab-174">Request</span></span>
<span data-ttu-id="980ab-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="980ab-175">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="980ab-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="980ab-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/schools/10002
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="980ab-177">C#</span><span class="sxs-lookup"><span data-stu-id="980ab-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="980ab-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="980ab-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="980ab-179">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="980ab-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="980ab-180">Java</span><span class="sxs-lookup"><span data-stu-id="980ab-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="980ab-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="980ab-181">Response</span></span>
<span data-ttu-id="980ab-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="980ab-182">The following is an example of the response.</span></span> 

><span data-ttu-id="980ab-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="980ab-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
