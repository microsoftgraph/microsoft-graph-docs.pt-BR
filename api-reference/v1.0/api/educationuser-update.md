---
title: Atualizar propriedades de educationUser
description: Atualize as propriedades de um objeto **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bba954e428bbc81a6d83dd17471ca24b66133e95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087506"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="f1b10-103">Atualizar propriedades de educationUser</span><span class="sxs-lookup"><span data-stu-id="f1b10-103">Update educationUser properties</span></span>

<span data-ttu-id="f1b10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1b10-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1b10-105">Atualize as propriedades de um objeto **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="f1b10-105">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1b10-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1b10-106">Permissions</span></span>
<span data-ttu-id="f1b10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1b10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1b10-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1b10-109">Permission type</span></span>      | <span data-ttu-id="f1b10-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1b10-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1b10-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1b10-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="f1b10-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1b10-112">Not supported.</span></span>  |
|<span data-ttu-id="f1b10-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1b10-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f1b10-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1b10-114">Not supported.</span></span>  |
|<span data-ttu-id="f1b10-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1b10-115">Application</span></span> | <span data-ttu-id="f1b10-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1b10-116">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1b10-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1b10-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f1b10-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b10-118">Request headers</span></span>
| <span data-ttu-id="f1b10-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1b10-119">Header</span></span>       | <span data-ttu-id="f1b10-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f1b10-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1b10-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1b10-121">Authorization</span></span>  | <span data-ttu-id="f1b10-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1b10-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f1b10-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1b10-124">Content-Type</span></span>  | <span data-ttu-id="f1b10-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1b10-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1b10-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b10-126">Request body</span></span>
<span data-ttu-id="f1b10-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f1b10-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f1b10-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f1b10-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f1b10-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f1b10-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f1b10-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1b10-130">Property</span></span>     | <span data-ttu-id="f1b10-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1b10-131">Type</span></span>   |<span data-ttu-id="f1b10-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1b10-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1b10-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f1b10-133">displayName</span></span>| <span data-ttu-id="f1b10-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1b10-134">String</span></span>| <span data-ttu-id="f1b10-135">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="f1b10-135">Display Name of User</span></span>|
|<span data-ttu-id="f1b10-136">givenName</span><span class="sxs-lookup"><span data-stu-id="f1b10-136">givenName</span></span>| <span data-ttu-id="f1b10-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1b10-137">String</span></span> | <span data-ttu-id="f1b10-138">Nome</span><span class="sxs-lookup"><span data-stu-id="f1b10-138">First Name</span></span> |
|<span data-ttu-id="f1b10-139">middleName</span><span class="sxs-lookup"><span data-stu-id="f1b10-139">middleName</span></span>| <span data-ttu-id="f1b10-140">String</span><span class="sxs-lookup"><span data-stu-id="f1b10-140">String</span></span> | <span data-ttu-id="f1b10-141">O nome do meio do usuário</span><span class="sxs-lookup"><span data-stu-id="f1b10-141">Middle Name of user</span></span>|
|<span data-ttu-id="f1b10-142">surname</span><span class="sxs-lookup"><span data-stu-id="f1b10-142">surname</span></span>| <span data-ttu-id="f1b10-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1b10-143">String</span></span> | <span data-ttu-id="f1b10-144">Sobrenome do usuário</span><span class="sxs-lookup"><span data-stu-id="f1b10-144">Surname of user</span></span>|
|<span data-ttu-id="f1b10-145">email</span><span class="sxs-lookup"><span data-stu-id="f1b10-145">mail</span></span>| <span data-ttu-id="f1b10-146">String</span><span class="sxs-lookup"><span data-stu-id="f1b10-146">String</span></span>| <span data-ttu-id="f1b10-147">endereço de email</span><span class="sxs-lookup"><span data-stu-id="f1b10-147">email address</span></span>|
|<span data-ttu-id="f1b10-148">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="f1b10-148">mobilePhone</span></span>| <span data-ttu-id="f1b10-149">String</span><span class="sxs-lookup"><span data-stu-id="f1b10-149">String</span></span> | <span data-ttu-id="f1b10-150">O número de celular do usuário</span><span class="sxs-lookup"><span data-stu-id="f1b10-150">Mobile number of user</span></span> |
|<span data-ttu-id="f1b10-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="f1b10-151">externalSource</span></span>|<span data-ttu-id="f1b10-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1b10-152">string</span></span>| <span data-ttu-id="f1b10-153">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="f1b10-153">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="f1b10-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="f1b10-154">externalSource</span></span>|<span data-ttu-id="f1b10-155">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1b10-155">string</span></span>| <span data-ttu-id="f1b10-156">De onde esse usuário foi criado.</span><span class="sxs-lookup"><span data-stu-id="f1b10-156">Where this user was created from.</span></span>  <span data-ttu-id="f1b10-157">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="f1b10-157">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="f1b10-158">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="f1b10-158">mailingAddress</span></span>|[<span data-ttu-id="f1b10-159">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f1b10-159">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="f1b10-160">Endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1b10-160">Mail address of user.</span></span>|
|<span data-ttu-id="f1b10-161">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="f1b10-161">residenceAddress</span></span>|[<span data-ttu-id="f1b10-162">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f1b10-162">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="f1b10-163">Endereço em que o usuário reside.</span><span class="sxs-lookup"><span data-stu-id="f1b10-163">Address where user lives.</span></span>|
|<span data-ttu-id="f1b10-164">primaryRole</span><span class="sxs-lookup"><span data-stu-id="f1b10-164">primaryRole</span></span>|<span data-ttu-id="f1b10-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1b10-165">string</span></span>| <span data-ttu-id="f1b10-166">Função padrão de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f1b10-166">Default Role for a user.</span></span>  <span data-ttu-id="f1b10-167">A função do usuário pode ser diferente em uma aula individual.</span><span class="sxs-lookup"><span data-stu-id="f1b10-167">The user's role might be different in an individual class.</span></span> <span data-ttu-id="f1b10-168">Os valores possíveis são: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="f1b10-168">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="f1b10-169">student</span><span class="sxs-lookup"><span data-stu-id="f1b10-169">student</span></span>|[<span data-ttu-id="f1b10-170">educationStudent</span><span class="sxs-lookup"><span data-stu-id="f1b10-170">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="f1b10-171">Se a função principal for aluno, esse bloco conterá dados específicos do aluno.</span><span class="sxs-lookup"><span data-stu-id="f1b10-171">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="f1b10-172">teacher</span><span class="sxs-lookup"><span data-stu-id="f1b10-172">teacher</span></span>|[<span data-ttu-id="f1b10-173">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="f1b10-173">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="f1b10-174">Se a função principal for professor, esse bloco conterá dados específicos do professor.</span><span class="sxs-lookup"><span data-stu-id="f1b10-174">If the primary role is teacher, this block will contain teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="f1b10-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1b10-175">Response</span></span>
<span data-ttu-id="f1b10-176">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1b10-176">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1b10-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1b10-177">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1b10-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b10-178">Request</span></span>
<span data-ttu-id="f1b10-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1b10-179">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1b10-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1b10-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/users/{user-id}
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
# <a name="c"></a>[<span data-ttu-id="f1b10-181">C#</span><span class="sxs-lookup"><span data-stu-id="f1b10-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1b10-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1b10-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1b10-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1b10-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1b10-184">Java</span><span class="sxs-lookup"><span data-stu-id="f1b10-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1b10-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1b10-185">Response</span></span>
<span data-ttu-id="f1b10-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1b10-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "student",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

