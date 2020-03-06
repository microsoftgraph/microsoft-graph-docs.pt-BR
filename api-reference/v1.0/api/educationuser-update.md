---
title: Atualizar propriedades de educationUser
description: Atualize as propriedades de um objeto **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 61c6293840c544e397f6761149c9131c94d9f930
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517401"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="c0549-103">Atualizar propriedades de educationUser</span><span class="sxs-lookup"><span data-stu-id="c0549-103">Update educationUser properties</span></span>

<span data-ttu-id="c0549-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0549-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0549-105">Atualize as propriedades de um objeto **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="c0549-105">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c0549-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0549-106">Permissions</span></span>
<span data-ttu-id="c0549-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0549-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0549-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0549-109">Permission type</span></span>      | <span data-ttu-id="c0549-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0549-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0549-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0549-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c0549-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0549-112">Not supported.</span></span>  |
|<span data-ttu-id="c0549-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0549-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c0549-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0549-114">Not supported.</span></span>  |
|<span data-ttu-id="c0549-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0549-115">Application</span></span> | <span data-ttu-id="c0549-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0549-116">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0549-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0549-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c0549-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0549-118">Request headers</span></span>
| <span data-ttu-id="c0549-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0549-119">Header</span></span>       | <span data-ttu-id="c0549-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c0549-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0549-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0549-121">Authorization</span></span>  | <span data-ttu-id="c0549-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0549-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c0549-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0549-124">Content-Type</span></span>  | <span data-ttu-id="c0549-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0549-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0549-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0549-126">Request body</span></span>
<span data-ttu-id="c0549-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c0549-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c0549-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="c0549-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c0549-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c0549-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c0549-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0549-130">Property</span></span>     | <span data-ttu-id="c0549-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0549-131">Type</span></span>   |<span data-ttu-id="c0549-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0549-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0549-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c0549-133">displayName</span></span>| <span data-ttu-id="c0549-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0549-134">String</span></span>| <span data-ttu-id="c0549-135">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="c0549-135">Display Name of User</span></span>|
|<span data-ttu-id="c0549-136">givenName</span><span class="sxs-lookup"><span data-stu-id="c0549-136">givenName</span></span>| <span data-ttu-id="c0549-137">String</span><span class="sxs-lookup"><span data-stu-id="c0549-137">String</span></span> | <span data-ttu-id="c0549-138">Nome</span><span class="sxs-lookup"><span data-stu-id="c0549-138">First Name</span></span> |
|<span data-ttu-id="c0549-139">middleName</span><span class="sxs-lookup"><span data-stu-id="c0549-139">middleName</span></span>| <span data-ttu-id="c0549-140">String</span><span class="sxs-lookup"><span data-stu-id="c0549-140">String</span></span> | <span data-ttu-id="c0549-141">O nome do meio do usuário</span><span class="sxs-lookup"><span data-stu-id="c0549-141">Middle Name of user</span></span>|
|<span data-ttu-id="c0549-142">surname</span><span class="sxs-lookup"><span data-stu-id="c0549-142">surname</span></span>| <span data-ttu-id="c0549-143">String</span><span class="sxs-lookup"><span data-stu-id="c0549-143">String</span></span> | <span data-ttu-id="c0549-144">Sobrenome do usuário</span><span class="sxs-lookup"><span data-stu-id="c0549-144">Surname of user</span></span>|
|<span data-ttu-id="c0549-145">email</span><span class="sxs-lookup"><span data-stu-id="c0549-145">mail</span></span>| <span data-ttu-id="c0549-146">String</span><span class="sxs-lookup"><span data-stu-id="c0549-146">String</span></span>| <span data-ttu-id="c0549-147">endereço de email</span><span class="sxs-lookup"><span data-stu-id="c0549-147">email address</span></span>|
|<span data-ttu-id="c0549-148">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="c0549-148">mobilePhone</span></span>| <span data-ttu-id="c0549-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0549-149">String</span></span> | <span data-ttu-id="c0549-150">O número de celular do usuário</span><span class="sxs-lookup"><span data-stu-id="c0549-150">Mobile number of user</span></span> |
|<span data-ttu-id="c0549-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="c0549-151">externalSource</span></span>|<span data-ttu-id="c0549-152">string</span><span class="sxs-lookup"><span data-stu-id="c0549-152">string</span></span>| <span data-ttu-id="c0549-153">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="c0549-153">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="c0549-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="c0549-154">externalSource</span></span>|<span data-ttu-id="c0549-155">string</span><span class="sxs-lookup"><span data-stu-id="c0549-155">string</span></span>| <span data-ttu-id="c0549-156">De onde esse usuário foi criado.</span><span class="sxs-lookup"><span data-stu-id="c0549-156">Where this user was created from.</span></span>  <span data-ttu-id="c0549-157">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="c0549-157">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="c0549-158">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="c0549-158">mailingAddress</span></span>|[<span data-ttu-id="c0549-159">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c0549-159">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="c0549-160">Endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="c0549-160">Mail address of user.</span></span>|
|<span data-ttu-id="c0549-161">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="c0549-161">residenceAddress</span></span>|[<span data-ttu-id="c0549-162">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c0549-162">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="c0549-163">Endereço em que o usuário reside.</span><span class="sxs-lookup"><span data-stu-id="c0549-163">Address where user lives.</span></span>|
|<span data-ttu-id="c0549-164">primaryRole</span><span class="sxs-lookup"><span data-stu-id="c0549-164">primaryRole</span></span>|<span data-ttu-id="c0549-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0549-165">string</span></span>| <span data-ttu-id="c0549-166">Função padrão de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c0549-166">Default Role for a user.</span></span>  <span data-ttu-id="c0549-167">A função do usuário pode ser diferente em uma aula individual.</span><span class="sxs-lookup"><span data-stu-id="c0549-167">The user's role might be different in an individual class.</span></span> <span data-ttu-id="c0549-168">Os valores possíveis são: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="c0549-168">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="c0549-169">student</span><span class="sxs-lookup"><span data-stu-id="c0549-169">student</span></span>|[<span data-ttu-id="c0549-170">educationStudent</span><span class="sxs-lookup"><span data-stu-id="c0549-170">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="c0549-171">Se a função principal for aluno, esse bloco conterá dados específicos do aluno.</span><span class="sxs-lookup"><span data-stu-id="c0549-171">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="c0549-172">teacher</span><span class="sxs-lookup"><span data-stu-id="c0549-172">teacher</span></span>|[<span data-ttu-id="c0549-173">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="c0549-173">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="c0549-174">Se a função principal for professor, esse bloco conterá dados específicos do professor.</span><span class="sxs-lookup"><span data-stu-id="c0549-174">If the primary role is teacher, this block will contain teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="c0549-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0549-175">Response</span></span>
<span data-ttu-id="c0549-176">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0549-176">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0549-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0549-177">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0549-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0549-178">Request</span></span>
<span data-ttu-id="c0549-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0549-179">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0549-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0549-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c0549-181">C#</span><span class="sxs-lookup"><span data-stu-id="c0549-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0549-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0549-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0549-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0549-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0549-184">Java</span><span class="sxs-lookup"><span data-stu-id="c0549-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0549-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0549-185">Response</span></span>
<span data-ttu-id="c0549-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0549-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
