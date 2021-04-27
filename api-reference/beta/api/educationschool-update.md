---
title: Atualizar propriedades educationSchool
description: Atualize as propriedades de um objeto de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bb25d6e2ff81542dcd5481215fd93687b388fe05
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043364"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="054ba-103">Atualizar as propriedades educationschool</span><span class="sxs-lookup"><span data-stu-id="054ba-103">Update educationschool properties</span></span>

<span data-ttu-id="054ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="054ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="054ba-105">Atualize as propriedades de um objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="054ba-105">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="054ba-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="054ba-106">Permissions</span></span>

<span data-ttu-id="054ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="054ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="054ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="054ba-109">Permission type</span></span>                        | <span data-ttu-id="054ba-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="054ba-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="054ba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="054ba-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="054ba-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="054ba-112">Not supported.</span></span>                              |
| <span data-ttu-id="054ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="054ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="054ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="054ba-114">Not supported.</span></span>                              |
| <span data-ttu-id="054ba-115">Application</span><span class="sxs-lookup"><span data-stu-id="054ba-115">Application</span></span>                            | <span data-ttu-id="054ba-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="054ba-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="054ba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="054ba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```

## <a name="request-headers"></a><span data-ttu-id="054ba-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="054ba-118">Request headers</span></span>

| <span data-ttu-id="054ba-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="054ba-119">Header</span></span>        | <span data-ttu-id="054ba-120">Valor</span><span class="sxs-lookup"><span data-stu-id="054ba-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="054ba-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="054ba-121">Authorization</span></span> | <span data-ttu-id="054ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="054ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="054ba-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="054ba-124">Content-Type</span></span>  | <span data-ttu-id="054ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="054ba-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="054ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="054ba-126">Request body</span></span>

<span data-ttu-id="054ba-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="054ba-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="054ba-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="054ba-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="054ba-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="054ba-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="054ba-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="054ba-130">Property</span></span>            | <span data-ttu-id="054ba-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="054ba-131">Type</span></span>                                               | <span data-ttu-id="054ba-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="054ba-132">Description</span></span>                        |
| :------------------ | :------------------------------------------------- | :--------------------------------- |
| <span data-ttu-id="054ba-133">displayName</span><span class="sxs-lookup"><span data-stu-id="054ba-133">displayName</span></span>         | <span data-ttu-id="054ba-134">String</span><span class="sxs-lookup"><span data-stu-id="054ba-134">String</span></span>                                             | <span data-ttu-id="054ba-135">Nome de exibição da escola</span><span class="sxs-lookup"><span data-stu-id="054ba-135">Display name of the school</span></span>         |
| <span data-ttu-id="054ba-136">description</span><span class="sxs-lookup"><span data-stu-id="054ba-136">description</span></span>         | <span data-ttu-id="054ba-137">String</span><span class="sxs-lookup"><span data-stu-id="054ba-137">String</span></span>                                             | <span data-ttu-id="054ba-138">Descrição da escola</span><span class="sxs-lookup"><span data-stu-id="054ba-138">Description of the school</span></span>          |
| <span data-ttu-id="054ba-139">principalEmail</span><span class="sxs-lookup"><span data-stu-id="054ba-139">principalEmail</span></span>      | <span data-ttu-id="054ba-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="054ba-140">String</span></span>                                             | <span data-ttu-id="054ba-141">Endereço de email da entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="054ba-141">Email address of the principal</span></span>     |
| <span data-ttu-id="054ba-142">principalName</span><span class="sxs-lookup"><span data-stu-id="054ba-142">principalName</span></span>       | <span data-ttu-id="054ba-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="054ba-143">String</span></span>                                             | <span data-ttu-id="054ba-144">Nome da entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="054ba-144">Name of the principal</span></span>              |
| <span data-ttu-id="054ba-145">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="054ba-145">externalPrincipalId</span></span> | <span data-ttu-id="054ba-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="054ba-146">String</span></span>                                             | <span data-ttu-id="054ba-147">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="054ba-147">Id of principal in syncing system.</span></span> |
| <span data-ttu-id="054ba-148">highestGrade</span><span class="sxs-lookup"><span data-stu-id="054ba-148">highestGrade</span></span>        | <span data-ttu-id="054ba-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="054ba-149">String</span></span>                                             | <span data-ttu-id="054ba-150">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="054ba-150">Highest grade taught.</span></span>              |
| <span data-ttu-id="054ba-151">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="054ba-151">lowestGrade</span></span>         | <span data-ttu-id="054ba-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="054ba-152">String</span></span>                                             | <span data-ttu-id="054ba-153">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="054ba-153">Lowest grade taught.</span></span>               |
| <span data-ttu-id="054ba-154">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="054ba-154">schoolNumber</span></span>        | <span data-ttu-id="054ba-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="054ba-155">String</span></span>                                             | <span data-ttu-id="054ba-156">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="054ba-156">School Number.</span></span>                     |
| <span data-ttu-id="054ba-157">externalId</span><span class="sxs-lookup"><span data-stu-id="054ba-157">externalId</span></span>          | <span data-ttu-id="054ba-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="054ba-158">String</span></span>                                             | <span data-ttu-id="054ba-159">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="054ba-159">Id of school in syncing system.</span></span>    |
| <span data-ttu-id="054ba-160">phone</span><span class="sxs-lookup"><span data-stu-id="054ba-160">phone</span></span>               | <span data-ttu-id="054ba-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="054ba-161">String</span></span>                                             | <span data-ttu-id="054ba-162">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="054ba-162">Phone number of school.</span></span>            |
| <span data-ttu-id="054ba-163">address</span><span class="sxs-lookup"><span data-stu-id="054ba-163">address</span></span>             | [<span data-ttu-id="054ba-164">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="054ba-164">physicalAddress</span></span>](../resources/physicaladdress.md) | <span data-ttu-id="054ba-165">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="054ba-165">Address of the School.</span></span>             |
| <span data-ttu-id="054ba-166">createdBy</span><span class="sxs-lookup"><span data-stu-id="054ba-166">createdBy</span></span>           | [<span data-ttu-id="054ba-167">identitySet</span><span class="sxs-lookup"><span data-stu-id="054ba-167">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="054ba-168">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="054ba-168">Entity who created the school.</span></span>     |

## <a name="response"></a><span data-ttu-id="054ba-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="054ba-169">Response</span></span>
<span data-ttu-id="054ba-170">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="054ba-170">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="054ba-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="054ba-171">Example</span></span>

##### <a name="request"></a><span data-ttu-id="054ba-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="054ba-172">Request</span></span>

<span data-ttu-id="054ba-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="054ba-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="054ba-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="054ba-174">HTTP</span></span>](#tab/http)

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
# <a name="c"></a>[<span data-ttu-id="054ba-175">C#</span><span class="sxs-lookup"><span data-stu-id="054ba-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]
# <a name="javascript"></a>[<span data-ttu-id="054ba-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="054ba-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]
# <a name="objective-c"></a>[<span data-ttu-id="054ba-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="054ba-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="054ba-178">Java</span><span class="sxs-lookup"><span data-stu-id="054ba-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="054ba-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="054ba-179">Response</span></span>

<span data-ttu-id="054ba-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="054ba-180">The following is an example of the response.</span></span>

><span data-ttu-id="054ba-181">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="054ba-181">**Note:** The response object shown here might be shortened for readability.</span></span>

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


