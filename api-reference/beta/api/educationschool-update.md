---
title: Atualizar propriedades de educationSchool
description: Atualize as propriedades de um objeto de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 52c5dc51edaebb0c5265af29990b548a490b1886
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2019
ms.locfileid: "37581186"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="40efa-103">Atualizar as propriedades educationschool</span><span class="sxs-lookup"><span data-stu-id="40efa-103">Update educationschool properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40efa-104">Atualize as propriedades de um objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="40efa-104">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40efa-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="40efa-105">Permissions</span></span>

<span data-ttu-id="40efa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40efa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40efa-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40efa-108">Permission type</span></span>                        | <span data-ttu-id="40efa-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40efa-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="40efa-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40efa-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="40efa-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40efa-111">Not supported.</span></span>                              |
| <span data-ttu-id="40efa-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40efa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40efa-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40efa-113">Not supported.</span></span>                              |
| <span data-ttu-id="40efa-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40efa-114">Application</span></span>                            | <span data-ttu-id="40efa-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40efa-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="40efa-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40efa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```

## <a name="request-headers"></a><span data-ttu-id="40efa-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40efa-117">Request headers</span></span>

| <span data-ttu-id="40efa-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40efa-118">Header</span></span>        | <span data-ttu-id="40efa-119">Valor</span><span class="sxs-lookup"><span data-stu-id="40efa-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="40efa-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="40efa-120">Authorization</span></span> | <span data-ttu-id="40efa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40efa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40efa-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40efa-123">Content-Type</span></span>  | <span data-ttu-id="40efa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="40efa-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="40efa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40efa-125">Request body</span></span>

<span data-ttu-id="40efa-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="40efa-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="40efa-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="40efa-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="40efa-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="40efa-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="40efa-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40efa-129">Property</span></span>            | <span data-ttu-id="40efa-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="40efa-130">Type</span></span>                                               | <span data-ttu-id="40efa-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="40efa-131">Description</span></span>                        |
| :------------------ | :------------------------------------------------- | :--------------------------------- |
| <span data-ttu-id="40efa-132">displayName</span><span class="sxs-lookup"><span data-stu-id="40efa-132">displayName</span></span>         | <span data-ttu-id="40efa-133">String</span><span class="sxs-lookup"><span data-stu-id="40efa-133">String</span></span>                                             | <span data-ttu-id="40efa-134">Nome de exibição da escola</span><span class="sxs-lookup"><span data-stu-id="40efa-134">Display name of the school</span></span>         |
| <span data-ttu-id="40efa-135">description</span><span class="sxs-lookup"><span data-stu-id="40efa-135">description</span></span>         | <span data-ttu-id="40efa-136">String</span><span class="sxs-lookup"><span data-stu-id="40efa-136">String</span></span>                                             | <span data-ttu-id="40efa-137">Descrição da escola</span><span class="sxs-lookup"><span data-stu-id="40efa-137">Description of the school</span></span>          |
| <span data-ttu-id="40efa-138">principalEmail</span><span class="sxs-lookup"><span data-stu-id="40efa-138">principalEmail</span></span>      | <span data-ttu-id="40efa-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40efa-139">String</span></span>                                             | <span data-ttu-id="40efa-140">Endereço de email da entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="40efa-140">Email address of the principal</span></span>     |
| <span data-ttu-id="40efa-141">principalName</span><span class="sxs-lookup"><span data-stu-id="40efa-141">principalName</span></span>       | <span data-ttu-id="40efa-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40efa-142">String</span></span>                                             | <span data-ttu-id="40efa-143">Nome da entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="40efa-143">Name of the principal</span></span>              |
| <span data-ttu-id="40efa-144">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="40efa-144">externalPrincipalId</span></span> | <span data-ttu-id="40efa-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40efa-145">String</span></span>                                             | <span data-ttu-id="40efa-146">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="40efa-146">Id of principal in syncing system.</span></span> |
| <span data-ttu-id="40efa-147">highestGrade</span><span class="sxs-lookup"><span data-stu-id="40efa-147">highestGrade</span></span>        | <span data-ttu-id="40efa-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40efa-148">String</span></span>                                             | <span data-ttu-id="40efa-149">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="40efa-149">Highest grade taught.</span></span>              |
| <span data-ttu-id="40efa-150">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="40efa-150">lowestGrade</span></span>         | <span data-ttu-id="40efa-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40efa-151">String</span></span>                                             | <span data-ttu-id="40efa-152">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="40efa-152">Lowest grade taught.</span></span>               |
| <span data-ttu-id="40efa-153">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="40efa-153">schoolNumber</span></span>        | <span data-ttu-id="40efa-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40efa-154">String</span></span>                                             | <span data-ttu-id="40efa-155">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="40efa-155">School Number.</span></span>                     |
| <span data-ttu-id="40efa-156">externalId</span><span class="sxs-lookup"><span data-stu-id="40efa-156">externalId</span></span>          | <span data-ttu-id="40efa-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40efa-157">String</span></span>                                             | <span data-ttu-id="40efa-158">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="40efa-158">Id of school in syncing system.</span></span>    |
| <span data-ttu-id="40efa-159">phone</span><span class="sxs-lookup"><span data-stu-id="40efa-159">phone</span></span>               | <span data-ttu-id="40efa-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40efa-160">String</span></span>                                             | <span data-ttu-id="40efa-161">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="40efa-161">Phone number of school.</span></span>            |
| <span data-ttu-id="40efa-162">address</span><span class="sxs-lookup"><span data-stu-id="40efa-162">address</span></span>             | [<span data-ttu-id="40efa-163">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="40efa-163">physicalAddress</span></span>](../resources/physicaladdress.md) | <span data-ttu-id="40efa-164">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="40efa-164">Address of the School.</span></span>             |
| <span data-ttu-id="40efa-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="40efa-165">createdBy</span></span>           | [<span data-ttu-id="40efa-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="40efa-166">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="40efa-167">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="40efa-167">Entity who created the school.</span></span>     |

## <a name="response"></a><span data-ttu-id="40efa-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="40efa-168">Response</span></span>
<span data-ttu-id="40efa-169">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40efa-169">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40efa-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40efa-170">Example</span></span>

##### <a name="request"></a><span data-ttu-id="40efa-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40efa-171">Request</span></span>

<span data-ttu-id="40efa-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="40efa-172">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="40efa-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="40efa-173">HTTP</span></span>](#tab/http)

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
# <a name="ctabcsharp"></a>[<span data-ttu-id="40efa-174">C#</span><span class="sxs-lookup"><span data-stu-id="40efa-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40efa-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40efa-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="40efa-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40efa-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="40efa-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="40efa-177">Response</span></span>

<span data-ttu-id="40efa-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="40efa-178">The following is an example of the response.</span></span>

><span data-ttu-id="40efa-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40efa-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
