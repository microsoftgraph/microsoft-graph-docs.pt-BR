---
title: Criar educationSchool
description: Crie um novo objeto educationSchool.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 98da82ad50ba9f1a8c8b5341730aa3b85f6345c0
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474810"
---
# <a name="create-educationschool"></a><span data-ttu-id="6330d-103">Criar educationSchool</span><span class="sxs-lookup"><span data-stu-id="6330d-103">Create educationSchool</span></span>

<span data-ttu-id="6330d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6330d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6330d-105">Crie um novo [objeto educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="6330d-105">Create a new [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6330d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6330d-106">Permissions</span></span>

<span data-ttu-id="6330d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6330d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6330d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6330d-109">Permission type</span></span>                        | <span data-ttu-id="6330d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6330d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6330d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6330d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6330d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6330d-112">Not supported.</span></span>                              |
| <span data-ttu-id="6330d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6330d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6330d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6330d-114">Not supported.</span></span>                              |
| <span data-ttu-id="6330d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6330d-115">Application</span></span>                            | <span data-ttu-id="6330d-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6330d-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="6330d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6330d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/schools
```

## <a name="request-headers"></a><span data-ttu-id="6330d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6330d-118">Request headers</span></span>

| <span data-ttu-id="6330d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6330d-119">Name</span></span>          | <span data-ttu-id="6330d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6330d-120">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="6330d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6330d-121">Authorization</span></span> | <span data-ttu-id="6330d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6330d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6330d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6330d-124">Content-Type</span></span>  | <span data-ttu-id="6330d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6330d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6330d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6330d-127">Request body</span></span>

<span data-ttu-id="6330d-128">No corpo da solicitação, fornece uma representação JSON do [objeto educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="6330d-128">In the request body, supply a JSON representation of the [educationSchool](../resources/educationschool.md) object.</span></span>

<span data-ttu-id="6330d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [a educationSchool](../resources/educationschool.md).</span><span class="sxs-lookup"><span data-stu-id="6330d-129">The following table shows the properties that are required when you create the [educationSchool](../resources/educationschool.md).</span></span>

| <span data-ttu-id="6330d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6330d-130">Property</span></span>             | <span data-ttu-id="6330d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6330d-131">Type</span></span>                                               | <span data-ttu-id="6330d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6330d-132">Description</span></span>                                                                                                                                                          |
| :------------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6330d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6330d-133">displayName</span></span>          | <span data-ttu-id="6330d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-134">String</span></span>                                             | <span data-ttu-id="6330d-135">Nome de exibição da escola.</span><span class="sxs-lookup"><span data-stu-id="6330d-135">Display name of the school.</span></span> <span data-ttu-id="6330d-136">Herdado de [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="6330d-136">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                           |
| <span data-ttu-id="6330d-137">descrição</span><span class="sxs-lookup"><span data-stu-id="6330d-137">description</span></span>          | <span data-ttu-id="6330d-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-138">String</span></span>                                             | <span data-ttu-id="6330d-139">Descrição da escola.</span><span class="sxs-lookup"><span data-stu-id="6330d-139">Description of the school.</span></span> <span data-ttu-id="6330d-140">Herdado de [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="6330d-140">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                            |
| <span data-ttu-id="6330d-141">externalSource</span><span class="sxs-lookup"><span data-stu-id="6330d-141">externalSource</span></span>       | <span data-ttu-id="6330d-142">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="6330d-142">educationExternalSource</span></span>                            | <span data-ttu-id="6330d-143">Fonte de onde essa organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="6330d-143">Source where this organization was created from.</span></span> <span data-ttu-id="6330d-144">Herdado de [educationOrganization](../resources/educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="6330d-144">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span> <span data-ttu-id="6330d-145">Os valores possíveis são: `sis` , 'manual.</span><span class="sxs-lookup"><span data-stu-id="6330d-145">Possible values are: `sis`, \`manual.</span></span> |
| <span data-ttu-id="6330d-146">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="6330d-146">externalSourceDetail</span></span> | <span data-ttu-id="6330d-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-147">String</span></span>                                             | <span data-ttu-id="6330d-148">O nome da fonte externa de onde esses recursos foram gerados.</span><span class="sxs-lookup"><span data-stu-id="6330d-148">The name of the external source this resources was generated from.</span></span>                                                                                                   |
| <span data-ttu-id="6330d-149">principalEmail</span><span class="sxs-lookup"><span data-stu-id="6330d-149">principalEmail</span></span>       | <span data-ttu-id="6330d-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-150">String</span></span>                                             | <span data-ttu-id="6330d-151">Endereço de email da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="6330d-151">Email address of the principal.</span></span>                                                                                                                                      |
| <span data-ttu-id="6330d-152">principalName</span><span class="sxs-lookup"><span data-stu-id="6330d-152">principalName</span></span>        | <span data-ttu-id="6330d-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-153">String</span></span>                                             | <span data-ttu-id="6330d-154">Nome da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="6330d-154">Name of the principal.</span></span>                                                                                                                                               |
| <span data-ttu-id="6330d-155">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="6330d-155">externalPrincipalId</span></span>  | <span data-ttu-id="6330d-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-156">String</span></span>                                             | <span data-ttu-id="6330d-157">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6330d-157">ID of principal in syncing system.</span></span>                                                                                                                                   |
| <span data-ttu-id="6330d-158">highestGrade</span><span class="sxs-lookup"><span data-stu-id="6330d-158">highestGrade</span></span>         | <span data-ttu-id="6330d-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-159">String</span></span>                                             | <span data-ttu-id="6330d-160">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="6330d-160">Highest grade taught.</span></span>                                                                                                                                                |
| <span data-ttu-id="6330d-161">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="6330d-161">lowestGrade</span></span>          | <span data-ttu-id="6330d-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-162">String</span></span>                                             | <span data-ttu-id="6330d-163">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="6330d-163">Lowest grade taught.</span></span>                                                                                                                                                 |
| <span data-ttu-id="6330d-164">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="6330d-164">schoolNumber</span></span>         | <span data-ttu-id="6330d-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-165">String</span></span>                                             | <span data-ttu-id="6330d-166">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="6330d-166">School Number.</span></span>                                                                                                                                                       |
| <span data-ttu-id="6330d-167">externalId</span><span class="sxs-lookup"><span data-stu-id="6330d-167">externalId</span></span>           | <span data-ttu-id="6330d-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-168">String</span></span>                                             | <span data-ttu-id="6330d-169">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="6330d-169">ID of school in syncing system.</span></span>                                                                                                                                      |
| <span data-ttu-id="6330d-170">phone</span><span class="sxs-lookup"><span data-stu-id="6330d-170">phone</span></span>                | <span data-ttu-id="6330d-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-171">String</span></span>                                             | <span data-ttu-id="6330d-172">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="6330d-172">Phone number of school.</span></span>                                                                                                                                              |
| <span data-ttu-id="6330d-173">fax</span><span class="sxs-lookup"><span data-stu-id="6330d-173">fax</span></span>                  | <span data-ttu-id="6330d-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330d-174">String</span></span>                                             | <span data-ttu-id="6330d-175">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="6330d-175">Fax number of school.</span></span>                                                                                                                                                |
| <span data-ttu-id="6330d-176">createdBy</span><span class="sxs-lookup"><span data-stu-id="6330d-176">createdBy</span></span>            | [<span data-ttu-id="6330d-177">identitySet</span><span class="sxs-lookup"><span data-stu-id="6330d-177">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="6330d-178">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="6330d-178">Entity who created the school.</span></span>                                                                                                                                       |
| <span data-ttu-id="6330d-179">address</span><span class="sxs-lookup"><span data-stu-id="6330d-179">address</span></span>              | [<span data-ttu-id="6330d-180">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="6330d-180">physicalAddress</span></span>](../resources/physicaladdress.md) | <span data-ttu-id="6330d-181">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="6330d-181">Address of the school.</span></span>                                                                                                                                               |

## <a name="response"></a><span data-ttu-id="6330d-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="6330d-182">Response</span></span>

<span data-ttu-id="6330d-183">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6330d-183">If successful, this method returns a `201 Created` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6330d-184">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6330d-184">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6330d-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6330d-185">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6330d-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="6330d-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/schools
Content-Type: application/json
Content-length: 583

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="6330d-187">C#</span><span class="sxs-lookup"><span data-stu-id="6330d-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationschool-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6330d-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6330d-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationschool-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6330d-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6330d-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationschool-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6330d-190">Java</span><span class="sxs-lookup"><span data-stu-id="6330d-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationschool-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6330d-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="6330d-191">Response</span></span>

> <span data-ttu-id="6330d-192">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6330d-192">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```
