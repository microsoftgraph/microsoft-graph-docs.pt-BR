---
title: Atualizar orgcontact
description: Atualize as propriedades do objeto orgcontact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d044d1d0add2887a690fa6e6b5ac3d00d9e9757
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450629"
---
# <a name="update-orgcontact"></a><span data-ttu-id="b1418-103">Atualizar orgcontact</span><span class="sxs-lookup"><span data-stu-id="b1418-103">Update orgcontact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1418-104">Atualize as propriedades do objeto orgcontact.</span><span class="sxs-lookup"><span data-stu-id="b1418-104">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1418-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1418-105">Permissions</span></span>
<span data-ttu-id="b1418-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1418-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1418-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1418-108">Permission type</span></span>      | <span data-ttu-id="b1418-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1418-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1418-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1418-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1418-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1418-111">Not supported.</span></span>    |
|<span data-ttu-id="b1418-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1418-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1418-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1418-113">Not supported.</span></span>    |
|<span data-ttu-id="b1418-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1418-114">Application</span></span> | <span data-ttu-id="b1418-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1418-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1418-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1418-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b1418-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1418-117">Request headers</span></span>
| <span data-ttu-id="b1418-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b1418-118">Name</span></span>       | <span data-ttu-id="b1418-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1418-119">Type</span></span> | <span data-ttu-id="b1418-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1418-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1418-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1418-121">Authorization</span></span>  | <span data-ttu-id="b1418-122">string</span><span class="sxs-lookup"><span data-stu-id="b1418-122">string</span></span>  | <span data-ttu-id="b1418-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1418-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1418-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1418-125">Request body</span></span>
<span data-ttu-id="b1418-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b1418-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b1418-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1418-129">Property</span></span>     | <span data-ttu-id="b1418-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1418-130">Type</span></span>   |<span data-ttu-id="b1418-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1418-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1418-132">city</span><span class="sxs-lookup"><span data-stu-id="b1418-132">city</span></span>|<span data-ttu-id="b1418-133">String</span><span class="sxs-lookup"><span data-stu-id="b1418-133">String</span></span>||
|<span data-ttu-id="b1418-134">country</span><span class="sxs-lookup"><span data-stu-id="b1418-134">country</span></span>|<span data-ttu-id="b1418-135">String</span><span class="sxs-lookup"><span data-stu-id="b1418-135">String</span></span>||
|<span data-ttu-id="b1418-136">department</span><span class="sxs-lookup"><span data-stu-id="b1418-136">department</span></span>|<span data-ttu-id="b1418-137">String</span><span class="sxs-lookup"><span data-stu-id="b1418-137">String</span></span>||
|<span data-ttu-id="b1418-138">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="b1418-138">onPremisesSyncEnabled</span></span>|<span data-ttu-id="b1418-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1418-139">Boolean</span></span>||
|<span data-ttu-id="b1418-140">displayName</span><span class="sxs-lookup"><span data-stu-id="b1418-140">displayName</span></span>|<span data-ttu-id="b1418-141">String</span><span class="sxs-lookup"><span data-stu-id="b1418-141">String</span></span>||
|<span data-ttu-id="b1418-142">givenName</span><span class="sxs-lookup"><span data-stu-id="b1418-142">givenName</span></span>|<span data-ttu-id="b1418-143">String</span><span class="sxs-lookup"><span data-stu-id="b1418-143">String</span></span>||
|<span data-ttu-id="b1418-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b1418-144">jobTitle</span></span>|<span data-ttu-id="b1418-145">String</span><span class="sxs-lookup"><span data-stu-id="b1418-145">String</span></span>||
|<span data-ttu-id="b1418-146">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b1418-146">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="b1418-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1418-147">DateTimeOffset</span></span>||
|<span data-ttu-id="b1418-148">email</span><span class="sxs-lookup"><span data-stu-id="b1418-148">mail</span></span>|<span data-ttu-id="b1418-149">String</span><span class="sxs-lookup"><span data-stu-id="b1418-149">String</span></span>||
|<span data-ttu-id="b1418-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b1418-150">mailNickname</span></span>|<span data-ttu-id="b1418-151">String</span><span class="sxs-lookup"><span data-stu-id="b1418-151">String</span></span>||
|<span data-ttu-id="b1418-152">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b1418-152">mobilePhone</span></span>|<span data-ttu-id="b1418-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1418-153">String</span></span>||
|<span data-ttu-id="b1418-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b1418-154">officeLocation</span></span>|<span data-ttu-id="b1418-155">String</span><span class="sxs-lookup"><span data-stu-id="b1418-155">String</span></span>||
|<span data-ttu-id="b1418-156">postalCode</span><span class="sxs-lookup"><span data-stu-id="b1418-156">postalCode</span></span>|<span data-ttu-id="b1418-157">String</span><span class="sxs-lookup"><span data-stu-id="b1418-157">String</span></span>||
|<span data-ttu-id="b1418-158">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="b1418-158">proxyAddresses</span></span>|<span data-ttu-id="b1418-159">String</span><span class="sxs-lookup"><span data-stu-id="b1418-159">String</span></span>||
|<span data-ttu-id="b1418-160">state</span><span class="sxs-lookup"><span data-stu-id="b1418-160">state</span></span>|<span data-ttu-id="b1418-161">String</span><span class="sxs-lookup"><span data-stu-id="b1418-161">String</span></span>||
|<span data-ttu-id="b1418-162">streetAddress</span><span class="sxs-lookup"><span data-stu-id="b1418-162">streetAddress</span></span>|<span data-ttu-id="b1418-163">String</span><span class="sxs-lookup"><span data-stu-id="b1418-163">String</span></span>||
|<span data-ttu-id="b1418-164">surname</span><span class="sxs-lookup"><span data-stu-id="b1418-164">surname</span></span>|<span data-ttu-id="b1418-165">String</span><span class="sxs-lookup"><span data-stu-id="b1418-165">String</span></span>||
|<span data-ttu-id="b1418-166">businessPhones</span><span class="sxs-lookup"><span data-stu-id="b1418-166">businessPhones</span></span>|<span data-ttu-id="b1418-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1418-167">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="b1418-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1418-168">Response</span></span>

<span data-ttu-id="b1418-169">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [orgContact](../resources/orgcontact.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1418-169">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1418-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1418-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1418-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1418-171">Request</span></span>
<span data-ttu-id="b1418-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1418-172">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b1418-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1418-173">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1418-174">C#</span><span class="sxs-lookup"><span data-stu-id="b1418-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1418-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="b1418-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1418-176">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b1418-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b1418-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1418-177">Response</span></span>
<span data-ttu-id="b1418-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1418-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
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
