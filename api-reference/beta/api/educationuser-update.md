---
title: Atualizar propriedades de educationUser
description: Atualize as propriedades de um objeto **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 4ba79c00d95764be03b98eac86d521debd808b19
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441167"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="3aacc-103">Atualizar propriedades de educationUser</span><span class="sxs-lookup"><span data-stu-id="3aacc-103">Update educationUser properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3aacc-104">Atualize as propriedades de um objeto **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="3aacc-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3aacc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3aacc-105">Permissions</span></span>
<span data-ttu-id="3aacc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aacc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aacc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3aacc-108">Permission type</span></span>      | <span data-ttu-id="3aacc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3aacc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3aacc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3aacc-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3aacc-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3aacc-111">Not supported.</span></span>  |
|<span data-ttu-id="3aacc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3aacc-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3aacc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3aacc-113">Not supported.</span></span>  |
|<span data-ttu-id="3aacc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3aacc-114">Application</span></span> | <span data-ttu-id="3aacc-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aacc-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3aacc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3aacc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3aacc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3aacc-117">Request headers</span></span>
| <span data-ttu-id="3aacc-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3aacc-118">Header</span></span>       | <span data-ttu-id="3aacc-119">Valor</span><span class="sxs-lookup"><span data-stu-id="3aacc-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3aacc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3aacc-120">Authorization</span></span>  | <span data-ttu-id="3aacc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3aacc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3aacc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3aacc-123">Content-Type</span></span>  | <span data-ttu-id="3aacc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3aacc-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3aacc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3aacc-125">Request body</span></span>
<span data-ttu-id="3aacc-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="3aacc-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="3aacc-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="3aacc-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3aacc-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3aacc-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3aacc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3aacc-129">Property</span></span>     | <span data-ttu-id="3aacc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3aacc-130">Type</span></span>   |<span data-ttu-id="3aacc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aacc-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3aacc-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3aacc-132">displayName</span></span>| <span data-ttu-id="3aacc-133">String</span><span class="sxs-lookup"><span data-stu-id="3aacc-133">String</span></span>| <span data-ttu-id="3aacc-134">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="3aacc-134">Display Name of User</span></span>|
|<span data-ttu-id="3aacc-135">givenName</span><span class="sxs-lookup"><span data-stu-id="3aacc-135">givenName</span></span>| <span data-ttu-id="3aacc-136">String</span><span class="sxs-lookup"><span data-stu-id="3aacc-136">String</span></span> | <span data-ttu-id="3aacc-137">Nome</span><span class="sxs-lookup"><span data-stu-id="3aacc-137">First Name</span></span> |
|<span data-ttu-id="3aacc-138">middleName</span><span class="sxs-lookup"><span data-stu-id="3aacc-138">middleName</span></span>| <span data-ttu-id="3aacc-139">String</span><span class="sxs-lookup"><span data-stu-id="3aacc-139">String</span></span> | <span data-ttu-id="3aacc-140">O nome do meio do usuário</span><span class="sxs-lookup"><span data-stu-id="3aacc-140">Middle Name of user</span></span>|
|<span data-ttu-id="3aacc-141">surname</span><span class="sxs-lookup"><span data-stu-id="3aacc-141">surname</span></span>| <span data-ttu-id="3aacc-142">String</span><span class="sxs-lookup"><span data-stu-id="3aacc-142">String</span></span> | <span data-ttu-id="3aacc-143">Sobrenome do usuário</span><span class="sxs-lookup"><span data-stu-id="3aacc-143">Surname of user</span></span>|
|<span data-ttu-id="3aacc-144">email</span><span class="sxs-lookup"><span data-stu-id="3aacc-144">mail</span></span>| <span data-ttu-id="3aacc-145">String</span><span class="sxs-lookup"><span data-stu-id="3aacc-145">String</span></span>| <span data-ttu-id="3aacc-146">endereço de email</span><span class="sxs-lookup"><span data-stu-id="3aacc-146">email address</span></span>|
|<span data-ttu-id="3aacc-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="3aacc-147">mobilePhone</span></span>| <span data-ttu-id="3aacc-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3aacc-148">String</span></span> | <span data-ttu-id="3aacc-149">O número de celular do usuário</span><span class="sxs-lookup"><span data-stu-id="3aacc-149">Mobile number of user</span></span> |
|<span data-ttu-id="3aacc-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="3aacc-150">externalSource</span></span>|<span data-ttu-id="3aacc-151">string</span><span class="sxs-lookup"><span data-stu-id="3aacc-151">string</span></span>| <span data-ttu-id="3aacc-152">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="3aacc-152">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="3aacc-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="3aacc-153">externalSource</span></span>|<span data-ttu-id="3aacc-154">string</span><span class="sxs-lookup"><span data-stu-id="3aacc-154">string</span></span>| <span data-ttu-id="3aacc-155">De onde esse usuário foi criado.</span><span class="sxs-lookup"><span data-stu-id="3aacc-155">Where this user was created from.</span></span>  <span data-ttu-id="3aacc-156">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="3aacc-156">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="3aacc-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="3aacc-157">mailingAddress</span></span>|[<span data-ttu-id="3aacc-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="3aacc-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="3aacc-159">Endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="3aacc-159">Mail address of user.</span></span>|
|<span data-ttu-id="3aacc-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="3aacc-160">residenceAddress</span></span>|[<span data-ttu-id="3aacc-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="3aacc-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="3aacc-162">Endereço em que o usuário reside.</span><span class="sxs-lookup"><span data-stu-id="3aacc-162">Address where user lives.</span></span>|
|<span data-ttu-id="3aacc-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="3aacc-163">primaryRole</span></span>|<span data-ttu-id="3aacc-164">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3aacc-164">string</span></span>| <span data-ttu-id="3aacc-165">Função padrão de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3aacc-165">Default Role for a user.</span></span>  <span data-ttu-id="3aacc-166">A função do usuário pode ser diferente em uma aula individual.</span><span class="sxs-lookup"><span data-stu-id="3aacc-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="3aacc-167">Os valores possíveis são: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="3aacc-167">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="3aacc-168">student</span><span class="sxs-lookup"><span data-stu-id="3aacc-168">student</span></span>|[<span data-ttu-id="3aacc-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="3aacc-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="3aacc-170">Se a função principal for aluno, esse bloco conterá dados específicos do aluno.</span><span class="sxs-lookup"><span data-stu-id="3aacc-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="3aacc-171">teacher</span><span class="sxs-lookup"><span data-stu-id="3aacc-171">teacher</span></span>|[<span data-ttu-id="3aacc-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="3aacc-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="3aacc-173">Se a função principal for professor, esse bloco conterá dados específicos do professor.</span><span class="sxs-lookup"><span data-stu-id="3aacc-173">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="3aacc-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aacc-174">Response</span></span>
<span data-ttu-id="3aacc-175">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aacc-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3aacc-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3aacc-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3aacc-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aacc-177">Request</span></span>
<span data-ttu-id="3aacc-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3aacc-178">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3aacc-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aacc-179">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3aacc-180">C#</span><span class="sxs-lookup"><span data-stu-id="3aacc-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3aacc-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="3aacc-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3aacc-182">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3aacc-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3aacc-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aacc-183">Response</span></span>
<span data-ttu-id="3aacc-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3aacc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
