---
title: Atualizar educationSchool
description: Atualize as propriedades de um objeto educationSchool.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e6c53b2b9b5934559a352378ee5316618ae69abe
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231868"
---
# <a name="update-educationschool"></a><span data-ttu-id="522f9-103">Atualizar educationSchool</span><span class="sxs-lookup"><span data-stu-id="522f9-103">Update educationSchool</span></span>

<span data-ttu-id="522f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="522f9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="522f9-105">Atualize as propriedades de um [objeto educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="522f9-105">Update the properties of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="522f9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="522f9-106">Permissions</span></span>

<span data-ttu-id="522f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="522f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="522f9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="522f9-109">Permission type</span></span>                        | <span data-ttu-id="522f9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="522f9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="522f9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="522f9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="522f9-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="522f9-112">Not supported.</span></span>                              |
| <span data-ttu-id="522f9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="522f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="522f9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="522f9-114">Not supported.</span></span>                              |
| <span data-ttu-id="522f9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="522f9-115">Application</span></span>                            | <span data-ttu-id="522f9-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="522f9-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="522f9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="522f9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```

## <a name="request-headers"></a><span data-ttu-id="522f9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="522f9-118">Request headers</span></span>

| <span data-ttu-id="522f9-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="522f9-119">Header</span></span>        | <span data-ttu-id="522f9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="522f9-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="522f9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="522f9-121">Authorization</span></span> | <span data-ttu-id="522f9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="522f9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="522f9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="522f9-124">Content-Type</span></span>  | <span data-ttu-id="522f9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="522f9-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="522f9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="522f9-126">Request body</span></span>

<span data-ttu-id="522f9-127">No corpo da solicitação, fornece uma representação JSON do [objeto educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="522f9-127">In the request body, supply a JSON representation of the [educationSchool](../resources/educationschool.md) object.</span></span>

<span data-ttu-id="522f9-128">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o educationSchool](../resources/educationschool.md).</span><span class="sxs-lookup"><span data-stu-id="522f9-128">The following table shows the properties that are required when you update the [educationSchool](../resources/educationschool.md).</span></span>

| <span data-ttu-id="522f9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="522f9-129">Property</span></span>             | <span data-ttu-id="522f9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="522f9-130">Type</span></span>                                               | <span data-ttu-id="522f9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="522f9-131">Description</span></span>                                                                                                                                                           |
| :------------------- | :------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="522f9-132">displayName</span><span class="sxs-lookup"><span data-stu-id="522f9-132">displayName</span></span>          | <span data-ttu-id="522f9-133">String</span><span class="sxs-lookup"><span data-stu-id="522f9-133">String</span></span>                                             | <span data-ttu-id="522f9-134">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="522f9-134">Display name of the school.</span></span> <span data-ttu-id="522f9-135">Herdado de [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="522f9-135">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                            |
| <span data-ttu-id="522f9-136">descrição</span><span class="sxs-lookup"><span data-stu-id="522f9-136">description</span></span>          | <span data-ttu-id="522f9-137">String</span><span class="sxs-lookup"><span data-stu-id="522f9-137">String</span></span>                                             | <span data-ttu-id="522f9-138">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="522f9-138">Description of the school.</span></span> <span data-ttu-id="522f9-139">Herdado de [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="522f9-139">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                             |
| <span data-ttu-id="522f9-140">externalSource</span><span class="sxs-lookup"><span data-stu-id="522f9-140">externalSource</span></span>       | <span data-ttu-id="522f9-141">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="522f9-141">educationExternalSource</span></span>                            | <span data-ttu-id="522f9-142">Fonte de onde essa organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="522f9-142">Source where this organization was created from.</span></span> <span data-ttu-id="522f9-143">Herdado de [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="522f9-143">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span> <span data-ttu-id="522f9-144">Os valores possíveis são: `sis` e `manual`.</span><span class="sxs-lookup"><span data-stu-id="522f9-144">Possible values are: `sis`, `manual`.</span></span> |
| <span data-ttu-id="522f9-145">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="522f9-145">externalSourceDetail</span></span> | <span data-ttu-id="522f9-146">String</span><span class="sxs-lookup"><span data-stu-id="522f9-146">String</span></span>                                             | <span data-ttu-id="522f9-147">O nome da fonte externa de onde esses recursos foram gerados.</span><span class="sxs-lookup"><span data-stu-id="522f9-147">The name of the external source this resources was generated from.</span></span>                                                                                                    |
| <span data-ttu-id="522f9-148">principalEmail</span><span class="sxs-lookup"><span data-stu-id="522f9-148">principalEmail</span></span>       | <span data-ttu-id="522f9-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522f9-149">String</span></span>                                             | <span data-ttu-id="522f9-150">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="522f9-150">Email address of the principal.</span></span>                                                                                                                                       |
| <span data-ttu-id="522f9-151">principalName</span><span class="sxs-lookup"><span data-stu-id="522f9-151">principalName</span></span>        | <span data-ttu-id="522f9-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522f9-152">String</span></span>                                             | <span data-ttu-id="522f9-153">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="522f9-153">Name of the principal.</span></span>                                                                                                                                                |
| <span data-ttu-id="522f9-154">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="522f9-154">externalPrincipalId</span></span>  | <span data-ttu-id="522f9-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522f9-155">String</span></span>                                             | <span data-ttu-id="522f9-156">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="522f9-156">ID of principal in syncing system.</span></span>                                                                                                                                    |
| <span data-ttu-id="522f9-157">highestGrade</span><span class="sxs-lookup"><span data-stu-id="522f9-157">highestGrade</span></span>         | <span data-ttu-id="522f9-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522f9-158">String</span></span>                                             | <span data-ttu-id="522f9-159">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="522f9-159">Highest grade taught.</span></span>                                                                                                                                                 |
| <span data-ttu-id="522f9-160">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="522f9-160">lowestGrade</span></span>          | <span data-ttu-id="522f9-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522f9-161">String</span></span>                                             | <span data-ttu-id="522f9-162">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="522f9-162">Lowest grade taught.</span></span>                                                                                                                                                  |
| <span data-ttu-id="522f9-163">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="522f9-163">schoolNumber</span></span>         | <span data-ttu-id="522f9-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522f9-164">String</span></span>                                             | <span data-ttu-id="522f9-165">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="522f9-165">School Number.</span></span>                                                                                                                                                        |
| <span data-ttu-id="522f9-166">externalId</span><span class="sxs-lookup"><span data-stu-id="522f9-166">externalId</span></span>           | <span data-ttu-id="522f9-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522f9-167">String</span></span>                                             | <span data-ttu-id="522f9-168">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="522f9-168">ID of school in syncing system.</span></span>                                                                                                                                       |
| <span data-ttu-id="522f9-169">phone</span><span class="sxs-lookup"><span data-stu-id="522f9-169">phone</span></span>                | <span data-ttu-id="522f9-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522f9-170">String</span></span>                                             | <span data-ttu-id="522f9-171">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="522f9-171">Phone number of school.</span></span>                                                                                                                                               |
| <span data-ttu-id="522f9-172">fax</span><span class="sxs-lookup"><span data-stu-id="522f9-172">fax</span></span>                  | <span data-ttu-id="522f9-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="522f9-173">String</span></span>                                             | <span data-ttu-id="522f9-174">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="522f9-174">Fax number of school.</span></span>                                                                                                                                                 |
| <span data-ttu-id="522f9-175">createdBy</span><span class="sxs-lookup"><span data-stu-id="522f9-175">createdBy</span></span>            | [<span data-ttu-id="522f9-176">identitySet</span><span class="sxs-lookup"><span data-stu-id="522f9-176">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="522f9-177">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="522f9-177">Entity who created the school.</span></span>                                                                                                                                        |
| <span data-ttu-id="522f9-178">address</span><span class="sxs-lookup"><span data-stu-id="522f9-178">address</span></span>              | [<span data-ttu-id="522f9-179">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="522f9-179">physicalAddress</span></span>](../resources/physicaladdress.md) | <span data-ttu-id="522f9-180">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="522f9-180">Address of the school.</span></span>                                                                                                                                                |

## <a name="response"></a><span data-ttu-id="522f9-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="522f9-181">Response</span></span>

<span data-ttu-id="522f9-182">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="522f9-182">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="522f9-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="522f9-183">Example</span></span>

##### <a name="request"></a><span data-ttu-id="522f9-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="522f9-184">Request</span></span>

<span data-ttu-id="522f9-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="522f9-185">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="522f9-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="522f9-186">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/{school-id}
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```

# <a name="c"></a>[<span data-ttu-id="522f9-187">C#</span><span class="sxs-lookup"><span data-stu-id="522f9-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="522f9-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="522f9-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="522f9-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="522f9-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="522f9-190">Java</span><span class="sxs-lookup"><span data-stu-id="522f9-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="522f9-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="522f9-191">Response</span></span>

<span data-ttu-id="522f9-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="522f9-192">The following is an example of the response.</span></span>

><span data-ttu-id="522f9-193">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="522f9-193">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
