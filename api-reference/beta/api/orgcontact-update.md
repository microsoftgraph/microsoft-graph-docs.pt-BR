---
title: Atualizar orgcontact
description: Atualize as propriedades do objeto orgcontact.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 85b08d815b742a0b4117c7dd0ae786da979f92dc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447818"
---
# <a name="update-orgcontact"></a><span data-ttu-id="6d162-103">Atualizar orgcontact</span><span class="sxs-lookup"><span data-stu-id="6d162-103">Update orgcontact</span></span>

<span data-ttu-id="6d162-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d162-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d162-105">Atualize as propriedades do objeto orgcontact.</span><span class="sxs-lookup"><span data-stu-id="6d162-105">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6d162-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d162-106">Permissions</span></span>
<span data-ttu-id="6d162-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d162-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d162-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d162-109">Permission type</span></span>      | <span data-ttu-id="6d162-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d162-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d162-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d162-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6d162-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d162-112">Not supported.</span></span>    |
|<span data-ttu-id="6d162-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d162-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d162-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d162-114">Not supported.</span></span>    |
|<span data-ttu-id="6d162-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d162-115">Application</span></span> | <span data-ttu-id="6d162-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d162-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d162-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d162-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6d162-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d162-118">Request headers</span></span>
| <span data-ttu-id="6d162-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6d162-119">Name</span></span>       | <span data-ttu-id="6d162-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d162-120">Type</span></span> | <span data-ttu-id="6d162-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d162-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6d162-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d162-122">Authorization</span></span>  | <span data-ttu-id="6d162-123">string</span><span class="sxs-lookup"><span data-stu-id="6d162-123">string</span></span>  | <span data-ttu-id="6d162-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d162-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d162-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d162-126">Request body</span></span>
<span data-ttu-id="6d162-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6d162-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6d162-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d162-130">Property</span></span>     | <span data-ttu-id="6d162-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d162-131">Type</span></span>   |<span data-ttu-id="6d162-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d162-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d162-133">city</span><span class="sxs-lookup"><span data-stu-id="6d162-133">city</span></span>|<span data-ttu-id="6d162-134">String</span><span class="sxs-lookup"><span data-stu-id="6d162-134">String</span></span>||
|<span data-ttu-id="6d162-135">country</span><span class="sxs-lookup"><span data-stu-id="6d162-135">country</span></span>|<span data-ttu-id="6d162-136">String</span><span class="sxs-lookup"><span data-stu-id="6d162-136">String</span></span>||
|<span data-ttu-id="6d162-137">department</span><span class="sxs-lookup"><span data-stu-id="6d162-137">department</span></span>|<span data-ttu-id="6d162-138">String</span><span class="sxs-lookup"><span data-stu-id="6d162-138">String</span></span>||
|<span data-ttu-id="6d162-139">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="6d162-139">onPremisesSyncEnabled</span></span>|<span data-ttu-id="6d162-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d162-140">Boolean</span></span>||
|<span data-ttu-id="6d162-141">displayName</span><span class="sxs-lookup"><span data-stu-id="6d162-141">displayName</span></span>|<span data-ttu-id="6d162-142">String</span><span class="sxs-lookup"><span data-stu-id="6d162-142">String</span></span>||
|<span data-ttu-id="6d162-143">givenName</span><span class="sxs-lookup"><span data-stu-id="6d162-143">givenName</span></span>|<span data-ttu-id="6d162-144">String</span><span class="sxs-lookup"><span data-stu-id="6d162-144">String</span></span>||
|<span data-ttu-id="6d162-145">jobTitle</span><span class="sxs-lookup"><span data-stu-id="6d162-145">jobTitle</span></span>|<span data-ttu-id="6d162-146">String</span><span class="sxs-lookup"><span data-stu-id="6d162-146">String</span></span>||
|<span data-ttu-id="6d162-147">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6d162-147">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="6d162-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d162-148">DateTimeOffset</span></span>||
|<span data-ttu-id="6d162-149">email</span><span class="sxs-lookup"><span data-stu-id="6d162-149">mail</span></span>|<span data-ttu-id="6d162-150">String</span><span class="sxs-lookup"><span data-stu-id="6d162-150">String</span></span>||
|<span data-ttu-id="6d162-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="6d162-151">mailNickname</span></span>|<span data-ttu-id="6d162-152">String</span><span class="sxs-lookup"><span data-stu-id="6d162-152">String</span></span>||
|<span data-ttu-id="6d162-153">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="6d162-153">mobilePhone</span></span>|<span data-ttu-id="6d162-154">String</span><span class="sxs-lookup"><span data-stu-id="6d162-154">String</span></span>||
|<span data-ttu-id="6d162-155">officeLocation</span><span class="sxs-lookup"><span data-stu-id="6d162-155">officeLocation</span></span>|<span data-ttu-id="6d162-156">String</span><span class="sxs-lookup"><span data-stu-id="6d162-156">String</span></span>||
|<span data-ttu-id="6d162-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="6d162-157">postalCode</span></span>|<span data-ttu-id="6d162-158">String</span><span class="sxs-lookup"><span data-stu-id="6d162-158">String</span></span>||
|<span data-ttu-id="6d162-159">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="6d162-159">proxyAddresses</span></span>|<span data-ttu-id="6d162-160">String</span><span class="sxs-lookup"><span data-stu-id="6d162-160">String</span></span>||
|<span data-ttu-id="6d162-161">state</span><span class="sxs-lookup"><span data-stu-id="6d162-161">state</span></span>|<span data-ttu-id="6d162-162">String</span><span class="sxs-lookup"><span data-stu-id="6d162-162">String</span></span>||
|<span data-ttu-id="6d162-163">streetAddress</span><span class="sxs-lookup"><span data-stu-id="6d162-163">streetAddress</span></span>|<span data-ttu-id="6d162-164">String</span><span class="sxs-lookup"><span data-stu-id="6d162-164">String</span></span>||
|<span data-ttu-id="6d162-165">surname</span><span class="sxs-lookup"><span data-stu-id="6d162-165">surname</span></span>|<span data-ttu-id="6d162-166">String</span><span class="sxs-lookup"><span data-stu-id="6d162-166">String</span></span>||
|<span data-ttu-id="6d162-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="6d162-167">businessPhones</span></span>|<span data-ttu-id="6d162-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d162-168">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="6d162-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d162-169">Response</span></span>

<span data-ttu-id="6d162-170">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6d162-170">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6d162-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d162-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d162-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d162-172">Request</span></span>
<span data-ttu-id="6d162-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d162-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d162-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d162-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}-->
```http
PATCH https://graph.microsoft.com/beta/contacts/{id}
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6d162-175">C#</span><span class="sxs-lookup"><span data-stu-id="6d162-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d162-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d162-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d162-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d162-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6d162-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d162-178">Response</span></span>
<span data-ttu-id="6d162-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6d162-179">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


