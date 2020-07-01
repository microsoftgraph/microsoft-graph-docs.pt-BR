---
title: Atualizar propriedades de educationUser
description: Atualize as propriedades de um objeto **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 022b30eb68b29f4a77c34b0a8dc588d6f4bba071
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006751"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="5ed43-103">Atualizar propriedades de educationUser</span><span class="sxs-lookup"><span data-stu-id="5ed43-103">Update educationUser properties</span></span>

<span data-ttu-id="5ed43-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ed43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ed43-105">Atualize as propriedades de um objeto **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="5ed43-105">Update the properties of an **educationuser** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ed43-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ed43-106">Permissions</span></span>

<span data-ttu-id="5ed43-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5ed43-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5ed43-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ed43-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ed43-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ed43-109">Permission type</span></span>                        | <span data-ttu-id="5ed43-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ed43-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5ed43-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ed43-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ed43-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ed43-112">Not supported.</span></span>                              |
| <span data-ttu-id="5ed43-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ed43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ed43-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ed43-114">Not supported.</span></span>                              |
| <span data-ttu-id="5ed43-115">Application</span><span class="sxs-lookup"><span data-stu-id="5ed43-115">Application</span></span>                            | <span data-ttu-id="5ed43-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ed43-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="5ed43-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ed43-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/me
PATCH /education/users/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5ed43-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ed43-118">Request headers</span></span>

| <span data-ttu-id="5ed43-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ed43-119">Header</span></span>        | <span data-ttu-id="5ed43-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5ed43-120">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="5ed43-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ed43-121">Authorization</span></span> | <span data-ttu-id="5ed43-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5ed43-122">Bearer {token}.</span></span> <span data-ttu-id="5ed43-123">Required.</span><span class="sxs-lookup"><span data-stu-id="5ed43-123">Required.</span></span>   |
| <span data-ttu-id="5ed43-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5ed43-124">Content-Type</span></span>  | <span data-ttu-id="5ed43-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="5ed43-125">application/json.</span></span> <span data-ttu-id="5ed43-126">Required.</span><span class="sxs-lookup"><span data-stu-id="5ed43-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ed43-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ed43-127">Request body</span></span>

<span data-ttu-id="5ed43-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="5ed43-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5ed43-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5ed43-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5ed43-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5ed43-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5ed43-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ed43-131">Property</span></span>         | <span data-ttu-id="5ed43-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ed43-132">Type</span></span>               | <span data-ttu-id="5ed43-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ed43-133">Description</span></span>                                                                                                                                     |
| :--------------- | :----------------- | :---------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5ed43-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5ed43-134">displayName</span></span>      | <span data-ttu-id="5ed43-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed43-135">String</span></span>             | <span data-ttu-id="5ed43-136">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="5ed43-136">Display Name of User</span></span>                                                                                                                            |
| <span data-ttu-id="5ed43-137">givenName</span><span class="sxs-lookup"><span data-stu-id="5ed43-137">givenName</span></span>        | <span data-ttu-id="5ed43-138">String</span><span class="sxs-lookup"><span data-stu-id="5ed43-138">String</span></span>             | <span data-ttu-id="5ed43-139">Nome</span><span class="sxs-lookup"><span data-stu-id="5ed43-139">First Name</span></span>                                                                                                                                      |
| <span data-ttu-id="5ed43-140">middleName</span><span class="sxs-lookup"><span data-stu-id="5ed43-140">middleName</span></span>       | <span data-ttu-id="5ed43-141">String</span><span class="sxs-lookup"><span data-stu-id="5ed43-141">String</span></span>             | <span data-ttu-id="5ed43-142">O nome do meio do usuário</span><span class="sxs-lookup"><span data-stu-id="5ed43-142">Middle Name of user</span></span>                                                                                                                             |
| <span data-ttu-id="5ed43-143">surname</span><span class="sxs-lookup"><span data-stu-id="5ed43-143">surname</span></span>          | <span data-ttu-id="5ed43-144">String</span><span class="sxs-lookup"><span data-stu-id="5ed43-144">String</span></span>             | <span data-ttu-id="5ed43-145">Sobrenome do usuário</span><span class="sxs-lookup"><span data-stu-id="5ed43-145">Surname of user</span></span>                                                                                                                                 |
| <span data-ttu-id="5ed43-146">email</span><span class="sxs-lookup"><span data-stu-id="5ed43-146">mail</span></span>             | <span data-ttu-id="5ed43-147">String</span><span class="sxs-lookup"><span data-stu-id="5ed43-147">String</span></span>             | <span data-ttu-id="5ed43-148">endereço de email</span><span class="sxs-lookup"><span data-stu-id="5ed43-148">email address</span></span>                                                                                                                                   |
| <span data-ttu-id="5ed43-149">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="5ed43-149">mobilePhone</span></span>      | <span data-ttu-id="5ed43-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed43-150">String</span></span>             | <span data-ttu-id="5ed43-151">O número de celular do usuário</span><span class="sxs-lookup"><span data-stu-id="5ed43-151">Mobile number of user</span></span>                                                                                                                           |
| <span data-ttu-id="5ed43-152">externalSource</span><span class="sxs-lookup"><span data-stu-id="5ed43-152">externalSource</span></span>   | <span data-ttu-id="5ed43-153">string</span><span class="sxs-lookup"><span data-stu-id="5ed43-153">string</span></span>             | <span data-ttu-id="5ed43-154">De onde esse usuário foi criado.</span><span class="sxs-lookup"><span data-stu-id="5ed43-154">Where this user was created from.</span></span> <span data-ttu-id="5ed43-155">Os valores possíveis são: `sis` , `manual` , ou `lms` .</span><span class="sxs-lookup"><span data-stu-id="5ed43-155">Possible values are: `sis`, `manual`, or `lms`.</span></span>                                                               |
| <span data-ttu-id="5ed43-156">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="5ed43-156">mailingAddress</span></span>   | <span data-ttu-id="5ed43-157">[physicalAddress]</span><span class="sxs-lookup"><span data-stu-id="5ed43-157">[physicalAddress]</span></span>  | <span data-ttu-id="5ed43-158">Endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ed43-158">Mail address of user.</span></span> <span data-ttu-id="5ed43-159">Observação: `type` e `postOfficeBox` não têm suporte para `educationUser` recursos.</span><span class="sxs-lookup"><span data-stu-id="5ed43-159">Note: `type` and `postOfficeBox` are not supported for `educationUser` resources.</span></span>                                         |
| <span data-ttu-id="5ed43-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="5ed43-160">residenceAddress</span></span> | <span data-ttu-id="5ed43-161">[physicalAddress]</span><span class="sxs-lookup"><span data-stu-id="5ed43-161">[physicalAddress]</span></span>  | <span data-ttu-id="5ed43-162">Endereço em que o usuário reside.</span><span class="sxs-lookup"><span data-stu-id="5ed43-162">Address where user lives.</span></span> <span data-ttu-id="5ed43-163">Observação: `type` e `postOfficeBox` não têm suporte para `educationUser` recursos.</span><span class="sxs-lookup"><span data-stu-id="5ed43-163">Note: `type` and `postOfficeBox` are not supported for `educationUser` resources.</span></span>                                     |
| <span data-ttu-id="5ed43-164">primaryRole</span><span class="sxs-lookup"><span data-stu-id="5ed43-164">primaryRole</span></span>      | <span data-ttu-id="5ed43-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ed43-165">string</span></span>             | <span data-ttu-id="5ed43-166">Função padrão de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5ed43-166">Default Role for a user.</span></span> <span data-ttu-id="5ed43-167">A função do usuário pode ser diferente em uma aula individual.</span><span class="sxs-lookup"><span data-stu-id="5ed43-167">The user's role might be different in an individual class.</span></span> <span data-ttu-id="5ed43-168">Os valores possíveis são: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="5ed43-168">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span> |
| <span data-ttu-id="5ed43-169">student</span><span class="sxs-lookup"><span data-stu-id="5ed43-169">student</span></span>          | <span data-ttu-id="5ed43-170">[educationStudent]</span><span class="sxs-lookup"><span data-stu-id="5ed43-170">[educationStudent]</span></span> | <span data-ttu-id="5ed43-171">Se a função principal for aluno, esse bloco conterá dados específicos do aluno.</span><span class="sxs-lookup"><span data-stu-id="5ed43-171">If the primary role is student, this block will contain student specific data.</span></span>                                                                  |
| <span data-ttu-id="5ed43-172">teacher</span><span class="sxs-lookup"><span data-stu-id="5ed43-172">teacher</span></span>          | [<span data-ttu-id="5ed43-173">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="5ed43-173">educationTeacher</span></span>](../resources/educationteacher.md) | <span data-ttu-id="5ed43-174">Se a função principal for professor, esse bloco conterá dados específicos do professor.</span><span class="sxs-lookup"><span data-stu-id="5ed43-174">If the primary role is teacher, this block will contain teacher specific data.</span></span>                                                                  |

## <a name="response"></a><span data-ttu-id="5ed43-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ed43-175">Response</span></span>

<span data-ttu-id="5ed43-176">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ed43-176">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ed43-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ed43-177">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5ed43-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ed43-178">Request</span></span>

<span data-ttu-id="5ed43-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ed43-179">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ed43-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ed43-180">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/users/13020
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```

# <a name="c"></a>[<span data-ttu-id="5ed43-181">C#</span><span class="sxs-lookup"><span data-stu-id="5ed43-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ed43-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ed43-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ed43-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ed43-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ed43-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ed43-184">Response</span></span>

<span data-ttu-id="5ed43-185">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="5ed43-185">Here is an example of the response.</span></span> <span data-ttu-id="5ed43-186">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="5ed43-186">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5ed43-187">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5ed43-187">All of the properties will be returned from an actual call.</span></span>

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
  "primaryRole": "string",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

[PhysicalAddress]: ../resources/physicaladdress.md
[physicaladdress]: ../resources/physicaladdress.md
[educationstudent]: ../resources/educationstudent.md
