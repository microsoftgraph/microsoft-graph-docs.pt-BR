---
title: Atualizar propriedades de educationUser
description: Atualize as propriedades de um objeto **educationuser**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 52b9e3f3784bae75ed9a2d4aa91fc52dd8917de6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976181"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="2fde3-103">Atualizar propriedades de educationUser</span><span class="sxs-lookup"><span data-stu-id="2fde3-103">Update educationUser properties</span></span>

> <span data-ttu-id="2fde3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2fde3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fde3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2fde3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2fde3-106">Atualize as propriedades de um objeto **educationuser**.</span><span class="sxs-lookup"><span data-stu-id="2fde3-106">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2fde3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fde3-107">Permissions</span></span>
<span data-ttu-id="2fde3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fde3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fde3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fde3-110">Permission type</span></span>      | <span data-ttu-id="2fde3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fde3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fde3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fde3-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="2fde3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fde3-113">Not supported.</span></span>  |
|<span data-ttu-id="2fde3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fde3-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2fde3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fde3-115">Not supported.</span></span>  |
|<span data-ttu-id="2fde3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fde3-116">Application</span></span> | <span data-ttu-id="2fde3-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fde3-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fde3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fde3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2fde3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fde3-119">Request headers</span></span>
| <span data-ttu-id="2fde3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2fde3-120">Header</span></span>       | <span data-ttu-id="2fde3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2fde3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2fde3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fde3-122">Authorization</span></span>  | <span data-ttu-id="2fde3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fde3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2fde3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2fde3-125">Content-Type</span></span>  | <span data-ttu-id="2fde3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fde3-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2fde3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fde3-127">Request body</span></span>
<span data-ttu-id="2fde3-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="2fde3-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2fde3-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="2fde3-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2fde3-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2fde3-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2fde3-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fde3-131">Property</span></span>     | <span data-ttu-id="2fde3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fde3-132">Type</span></span>   |<span data-ttu-id="2fde3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fde3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fde3-134">displayName</span><span class="sxs-lookup"><span data-stu-id="2fde3-134">displayName</span></span>| <span data-ttu-id="2fde3-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fde3-135">String</span></span>| <span data-ttu-id="2fde3-136">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="2fde3-136">Display Name of User</span></span>|
|<span data-ttu-id="2fde3-137">givenName</span><span class="sxs-lookup"><span data-stu-id="2fde3-137">givenName</span></span>| <span data-ttu-id="2fde3-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fde3-138">String</span></span> | <span data-ttu-id="2fde3-139">Nome</span><span class="sxs-lookup"><span data-stu-id="2fde3-139">First Name</span></span> |
|<span data-ttu-id="2fde3-140">middleName</span><span class="sxs-lookup"><span data-stu-id="2fde3-140">middleName</span></span>| <span data-ttu-id="2fde3-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fde3-141">String</span></span> | <span data-ttu-id="2fde3-142">O nome do meio do usuário</span><span class="sxs-lookup"><span data-stu-id="2fde3-142">Middle Name of user</span></span>|
|<span data-ttu-id="2fde3-143">surname</span><span class="sxs-lookup"><span data-stu-id="2fde3-143">surname</span></span>| <span data-ttu-id="2fde3-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fde3-144">String</span></span> | <span data-ttu-id="2fde3-145">Sobrenome do usuário</span><span class="sxs-lookup"><span data-stu-id="2fde3-145">Surname of user</span></span>|
|<span data-ttu-id="2fde3-146">mail</span><span class="sxs-lookup"><span data-stu-id="2fde3-146">mail</span></span>| <span data-ttu-id="2fde3-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fde3-147">String</span></span>| <span data-ttu-id="2fde3-148">endereço de email</span><span class="sxs-lookup"><span data-stu-id="2fde3-148">email address</span></span>|
|<span data-ttu-id="2fde3-149">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="2fde3-149">mobilePhone</span></span>| <span data-ttu-id="2fde3-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fde3-150">String</span></span> | <span data-ttu-id="2fde3-151">O número de celular do usuário</span><span class="sxs-lookup"><span data-stu-id="2fde3-151">Mobile number of user</span></span> |
|<span data-ttu-id="2fde3-152">externalSource</span><span class="sxs-lookup"><span data-stu-id="2fde3-152">externalSource</span></span>|<span data-ttu-id="2fde3-153">string</span><span class="sxs-lookup"><span data-stu-id="2fde3-153">string</span></span>| <span data-ttu-id="2fde3-154">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="2fde3-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="2fde3-155">externalSource</span><span class="sxs-lookup"><span data-stu-id="2fde3-155">externalSource</span></span>|<span data-ttu-id="2fde3-156">string</span><span class="sxs-lookup"><span data-stu-id="2fde3-156">string</span></span>| <span data-ttu-id="2fde3-157">De onde esse usuário foi criado.</span><span class="sxs-lookup"><span data-stu-id="2fde3-157">Where this user was created from.</span></span>  <span data-ttu-id="2fde3-158">Os valores possíveis são: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="2fde3-158">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="2fde3-159">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="2fde3-159">mailingAddress</span></span>|[<span data-ttu-id="2fde3-160">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2fde3-160">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="2fde3-161">Endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="2fde3-161">Mail address of user.</span></span>|
|<span data-ttu-id="2fde3-162">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="2fde3-162">residenceAddress</span></span>|[<span data-ttu-id="2fde3-163">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="2fde3-163">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="2fde3-164">Endereço em que o usuário reside.</span><span class="sxs-lookup"><span data-stu-id="2fde3-164">Address where user lives.</span></span>|
|<span data-ttu-id="2fde3-165">primaryRole</span><span class="sxs-lookup"><span data-stu-id="2fde3-165">primaryRole</span></span>|<span data-ttu-id="2fde3-166">string</span><span class="sxs-lookup"><span data-stu-id="2fde3-166">string</span></span>| <span data-ttu-id="2fde3-167">Função padrão de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2fde3-167">Default Role for a user.</span></span>  <span data-ttu-id="2fde3-168">A função do usuário pode ser diferente em uma aula individual.</span><span class="sxs-lookup"><span data-stu-id="2fde3-168">The user's role might be different in an individual class.</span></span> <span data-ttu-id="2fde3-169">Os valores possíveis são: `student`, `teacher`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="2fde3-169">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="2fde3-170">student</span><span class="sxs-lookup"><span data-stu-id="2fde3-170">student</span></span>|[<span data-ttu-id="2fde3-171">educationStudent</span><span class="sxs-lookup"><span data-stu-id="2fde3-171">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="2fde3-172">Se a função principal for aluno, esse bloco conterá dados específicos do aluno.</span><span class="sxs-lookup"><span data-stu-id="2fde3-172">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="2fde3-173">teacher</span><span class="sxs-lookup"><span data-stu-id="2fde3-173">teacher</span></span>|[<span data-ttu-id="2fde3-174">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="2fde3-174">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="2fde3-175">Se a função principal for professor, esse bloco conterá dados específicos do professor.</span><span class="sxs-lookup"><span data-stu-id="2fde3-175">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="2fde3-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fde3-176">Response</span></span>
<span data-ttu-id="2fde3-177">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fde3-177">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2fde3-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fde3-178">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2fde3-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fde3-179">Request</span></span>
<span data-ttu-id="2fde3-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fde3-180">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2fde3-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fde3-181">Response</span></span>
<span data-ttu-id="2fde3-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fde3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
