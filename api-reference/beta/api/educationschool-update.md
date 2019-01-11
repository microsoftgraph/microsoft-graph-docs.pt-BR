---
title: Atualizar as propriedades educationschool
description: Atualize as propriedades de um objeto de escola.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 23c7c476e2447fbde43a0e7521d4b3d626f80f5b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892229"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="7f94b-103">Atualizar as propriedades educationschool</span><span class="sxs-lookup"><span data-stu-id="7f94b-103">Update educationschool properties</span></span>

> <span data-ttu-id="7f94b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7f94b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f94b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7f94b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f94b-106">Atualize as propriedades de um objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="7f94b-106">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f94b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f94b-107">Permissions</span></span>
<span data-ttu-id="7f94b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f94b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f94b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f94b-110">Permission type</span></span>      | <span data-ttu-id="7f94b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f94b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f94b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f94b-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="7f94b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f94b-113">Not supported.</span></span>  |
|<span data-ttu-id="7f94b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f94b-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7f94b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f94b-115">Not supported.</span></span>  |
|<span data-ttu-id="7f94b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f94b-116">Application</span></span> | <span data-ttu-id="7f94b-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f94b-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f94b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f94b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7f94b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f94b-119">Request headers</span></span>
| <span data-ttu-id="7f94b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f94b-120">Header</span></span>       | <span data-ttu-id="7f94b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7f94b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7f94b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f94b-122">Authorization</span></span>  | <span data-ttu-id="7f94b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f94b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7f94b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f94b-125">Content-Type</span></span>  | <span data-ttu-id="7f94b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f94b-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f94b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f94b-127">Request body</span></span>
<span data-ttu-id="7f94b-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="7f94b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7f94b-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="7f94b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7f94b-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="7f94b-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7f94b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f94b-131">Property</span></span>     | <span data-ttu-id="7f94b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f94b-132">Type</span></span>   |<span data-ttu-id="7f94b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f94b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f94b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="7f94b-134">displayName</span></span>| <span data-ttu-id="7f94b-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f94b-135">String</span></span>| <span data-ttu-id="7f94b-136">Nome de exibição da escola</span><span class="sxs-lookup"><span data-stu-id="7f94b-136">Display name of the school</span></span>| 
|<span data-ttu-id="7f94b-137">description</span><span class="sxs-lookup"><span data-stu-id="7f94b-137">description</span></span>| <span data-ttu-id="7f94b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f94b-138">String</span></span> | <span data-ttu-id="7f94b-139">Descrição da escola</span><span class="sxs-lookup"><span data-stu-id="7f94b-139">Description of the school</span></span>| 
|<span data-ttu-id="7f94b-140">principalEmail</span><span class="sxs-lookup"><span data-stu-id="7f94b-140">principalEmail</span></span>| <span data-ttu-id="7f94b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f94b-141">String</span></span>| <span data-ttu-id="7f94b-142">Endereço de email da entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="7f94b-142">Email address of the principal</span></span>|
|<span data-ttu-id="7f94b-143">principalName</span><span class="sxs-lookup"><span data-stu-id="7f94b-143">principalName</span></span>| <span data-ttu-id="7f94b-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f94b-144">String</span></span> | <span data-ttu-id="7f94b-145">Nome da entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="7f94b-145">Name of the principal</span></span>|
|<span data-ttu-id="7f94b-146">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="7f94b-146">externalPrincipalId</span></span>| <span data-ttu-id="7f94b-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f94b-147">String</span></span> | <span data-ttu-id="7f94b-148">ID da entidade de segurança no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7f94b-148">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="7f94b-149">highestGrade</span><span class="sxs-lookup"><span data-stu-id="7f94b-149">highestGrade</span></span>|<span data-ttu-id="7f94b-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f94b-150">String</span></span>| <span data-ttu-id="7f94b-151">Ensino de nível mais alto.</span><span class="sxs-lookup"><span data-stu-id="7f94b-151">Highest grade taught.</span></span> |
|<span data-ttu-id="7f94b-152">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="7f94b-152">lowestGrade</span></span>|<span data-ttu-id="7f94b-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f94b-153">String</span></span>| <span data-ttu-id="7f94b-154">Ensino de nível mais baixo.</span><span class="sxs-lookup"><span data-stu-id="7f94b-154">Lowest grade taught.</span></span> |
|<span data-ttu-id="7f94b-155">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="7f94b-155">schoolNumber</span></span>|<span data-ttu-id="7f94b-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f94b-156">String</span></span>| <span data-ttu-id="7f94b-157">Número da escola.</span><span class="sxs-lookup"><span data-stu-id="7f94b-157">School Number.</span></span>|
|<span data-ttu-id="7f94b-158">externalId</span><span class="sxs-lookup"><span data-stu-id="7f94b-158">externalId</span></span>|<span data-ttu-id="7f94b-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f94b-159">String</span></span>| <span data-ttu-id="7f94b-160">ID da escola no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7f94b-160">Id of school in syncing system.</span></span> |
|<span data-ttu-id="7f94b-161">phone</span><span class="sxs-lookup"><span data-stu-id="7f94b-161">phone</span></span>|<span data-ttu-id="7f94b-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f94b-162">String</span></span>| <span data-ttu-id="7f94b-163">Número de telefone da escola.</span><span class="sxs-lookup"><span data-stu-id="7f94b-163">Phone number of school.</span></span> |
|<span data-ttu-id="7f94b-164">fax</span><span class="sxs-lookup"><span data-stu-id="7f94b-164">fax</span></span>|<span data-ttu-id="7f94b-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f94b-165">String</span></span>| <span data-ttu-id="7f94b-166">Número de fax da escola.</span><span class="sxs-lookup"><span data-stu-id="7f94b-166">Fax number of school.</span></span> |
|<span data-ttu-id="7f94b-167">address</span><span class="sxs-lookup"><span data-stu-id="7f94b-167">address</span></span>|[<span data-ttu-id="7f94b-168">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="7f94b-168">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="7f94b-169">Endereço da escola.</span><span class="sxs-lookup"><span data-stu-id="7f94b-169">Address of the School.</span></span>|
|<span data-ttu-id="7f94b-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="7f94b-170">createdBy</span></span>|[<span data-ttu-id="7f94b-171">identitySet</span><span class="sxs-lookup"><span data-stu-id="7f94b-171">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="7f94b-172">Entidade que criou a escola.</span><span class="sxs-lookup"><span data-stu-id="7f94b-172">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="7f94b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f94b-173">Response</span></span>
<span data-ttu-id="7f94b-174">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f94b-174">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f94b-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f94b-175">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f94b-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f94b-176">Request</span></span>
<span data-ttu-id="7f94b-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f94b-177">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="7f94b-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f94b-178">Response</span></span>
<span data-ttu-id="7f94b-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f94b-179">The following is an example of the response.</span></span> 

><span data-ttu-id="7f94b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f94b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "fax": "+1 (253) 555-0101",
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
  "tocPath": ""
}-->
