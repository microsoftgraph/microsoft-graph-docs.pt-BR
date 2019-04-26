---
title: Atualizar propriedades de educationUser
description: Atualize as propriedades de um objeto **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: ef544aca0509322d12d6cd3e70e4c52334272bb3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324829"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="2dbe4-103">Atualizar propriedades de educationUser</span><span class="sxs-lookup"><span data-stu-id="2dbe4-103">Update educationUser properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dbe4-104">Atualize as propriedades de um objeto **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2dbe4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2dbe4-105">Permissions</span></span>
<span data-ttu-id="2dbe4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dbe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dbe4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2dbe4-108">Permission type</span></span>      | <span data-ttu-id="2dbe4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2dbe4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dbe4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2dbe4-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2dbe4-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-111">Not supported.</span></span>  |
|<span data-ttu-id="2dbe4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2dbe4-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2dbe4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-113">Not supported.</span></span>  |
|<span data-ttu-id="2dbe4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2dbe4-114">Application</span></span> | <span data-ttu-id="2dbe4-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dbe4-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2dbe4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2dbe4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2dbe4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2dbe4-117">Request headers</span></span>
| <span data-ttu-id="2dbe4-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2dbe4-118">Header</span></span>       | <span data-ttu-id="2dbe4-119">Valor</span><span class="sxs-lookup"><span data-stu-id="2dbe4-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2dbe4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2dbe4-120">Authorization</span></span>  | <span data-ttu-id="2dbe4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2dbe4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2dbe4-123">Content-Type</span></span>  | <span data-ttu-id="2dbe4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2dbe4-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2dbe4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2dbe4-125">Request body</span></span>
<span data-ttu-id="2dbe4-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2dbe4-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2dbe4-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2dbe4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2dbe4-129">Property</span></span>     | <span data-ttu-id="2dbe4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dbe4-130">Type</span></span>   |<span data-ttu-id="2dbe4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dbe4-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dbe4-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2dbe4-132">displayName</span></span>| <span data-ttu-id="2dbe4-133">String</span><span class="sxs-lookup"><span data-stu-id="2dbe4-133">String</span></span>| <span data-ttu-id="2dbe4-134">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="2dbe4-134">Display Name of User</span></span>|
|<span data-ttu-id="2dbe4-135">givenName</span><span class="sxs-lookup"><span data-stu-id="2dbe4-135">givenName</span></span>| <span data-ttu-id="2dbe4-136">String</span><span class="sxs-lookup"><span data-stu-id="2dbe4-136">String</span></span> | <span data-ttu-id="2dbe4-137">Nome</span><span class="sxs-lookup"><span data-stu-id="2dbe4-137">First Name</span></span> |
|<span data-ttu-id="2dbe4-138">middleName</span><span class="sxs-lookup"><span data-stu-id="2dbe4-138">middleName</span></span>| <span data-ttu-id="2dbe4-139">String</span><span class="sxs-lookup"><span data-stu-id="2dbe4-139">String</span></span> | <span data-ttu-id="2dbe4-140">O nome do meio do usuário</span><span class="sxs-lookup"><span data-stu-id="2dbe4-140">Middle Name of user</span></span>|
|<span data-ttu-id="2dbe4-141">surname</span><span class="sxs-lookup"><span data-stu-id="2dbe4-141">surname</span></span>| <span data-ttu-id="2dbe4-142">String</span><span class="sxs-lookup"><span data-stu-id="2dbe4-142">String</span></span> | <span data-ttu-id="2dbe4-143">Sobrenome do usuário</span><span class="sxs-lookup"><span data-stu-id="2dbe4-143">Surname of user</span></span>|
|<span data-ttu-id="2dbe4-144">email</span><span class="sxs-lookup"><span data-stu-id="2dbe4-144">mail</span></span>| <span data-ttu-id="2dbe4-145">String</span><span class="sxs-lookup"><span data-stu-id="2dbe4-145">String</span></span>| <span data-ttu-id="2dbe4-146">endereço de email</span><span class="sxs-lookup"><span data-stu-id="2dbe4-146">email address</span></span>|
|<span data-ttu-id="2dbe4-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="2dbe4-147">mobilePhone</span></span>| <span data-ttu-id="2dbe4-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2dbe4-148">String</span></span> | <span data-ttu-id="2dbe4-149">O número de celular do usuário</span><span class="sxs-lookup"><span data-stu-id="2dbe4-149">Mobile number of user</span></span> |
|<span data-ttu-id="2dbe4-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="2dbe4-150">externalSource</span></span>|<span data-ttu-id="2dbe4-151">string</span><span class="sxs-lookup"><span data-stu-id="2dbe4-151">string</span></span>| <span data-ttu-id="2dbe4-152">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-152">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="2dbe4-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="2dbe4-153">externalSource</span></span>|<span data-ttu-id="2dbe4-154">string</span><span class="sxs-lookup"><span data-stu-id="2dbe4-154">string</span></span>| <span data-ttu-id="2dbe4-155">De onde esse usuário foi criado.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-155">Where this user was created from.</span></span>  <span data-ttu-id="2dbe4-156">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-156">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="2dbe4-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="2dbe4-157">mailingAddress</span></span>|[<span data-ttu-id="2dbe4-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2dbe4-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="2dbe4-159">Endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-159">Mail address of user.</span></span>|
|<span data-ttu-id="2dbe4-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="2dbe4-160">residenceAddress</span></span>|[<span data-ttu-id="2dbe4-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2dbe4-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="2dbe4-162">Endereço em que o usuário reside.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-162">Address where user lives.</span></span>|
|<span data-ttu-id="2dbe4-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="2dbe4-163">primaryRole</span></span>|<span data-ttu-id="2dbe4-164">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2dbe4-164">string</span></span>| <span data-ttu-id="2dbe4-165">Função padrão de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-165">Default Role for a user.</span></span>  <span data-ttu-id="2dbe4-166">A função do usuário pode ser diferente em uma aula individual.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="2dbe4-167">Os valores possíveis são: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-167">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="2dbe4-168">student</span><span class="sxs-lookup"><span data-stu-id="2dbe4-168">student</span></span>|[<span data-ttu-id="2dbe4-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="2dbe4-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="2dbe4-170">Se a função principal for aluno, esse bloco conterá dados específicos do aluno.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="2dbe4-171">teacher</span><span class="sxs-lookup"><span data-stu-id="2dbe4-171">teacher</span></span>|[<span data-ttu-id="2dbe4-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="2dbe4-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="2dbe4-173">Se a função principal for professor, esse bloco conterá dados específicos do professor.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-173">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="2dbe4-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dbe4-174">Response</span></span>
<span data-ttu-id="2dbe4-175">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2dbe4-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2dbe4-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2dbe4-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2dbe4-177">Request</span></span>
<span data-ttu-id="2dbe4-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-178">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2dbe4-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dbe4-179">Response</span></span>
<span data-ttu-id="2dbe4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2dbe4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
