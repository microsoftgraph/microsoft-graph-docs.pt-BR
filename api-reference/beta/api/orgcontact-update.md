---
title: Atualizar orgcontact
description: Atualize as propriedades do objeto orgcontact.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 959be23764b5348c0e9473aa00205620f321ebb4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596596"
---
# <a name="update-orgcontact"></a><span data-ttu-id="083fe-103">Atualizar orgcontact</span><span class="sxs-lookup"><span data-stu-id="083fe-103">Update orgcontact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="083fe-104">Atualize as propriedades do objeto orgcontact.</span><span class="sxs-lookup"><span data-stu-id="083fe-104">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="083fe-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="083fe-105">Permissions</span></span>
<span data-ttu-id="083fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="083fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="083fe-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="083fe-108">Permission type</span></span>      | <span data-ttu-id="083fe-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="083fe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="083fe-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="083fe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="083fe-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="083fe-111">Not supported.</span></span>    |
|<span data-ttu-id="083fe-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="083fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="083fe-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="083fe-113">Not supported.</span></span>    |
|<span data-ttu-id="083fe-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="083fe-114">Application</span></span> | <span data-ttu-id="083fe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="083fe-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="083fe-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="083fe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="083fe-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="083fe-117">Request headers</span></span>
| <span data-ttu-id="083fe-118">Nome</span><span class="sxs-lookup"><span data-stu-id="083fe-118">Name</span></span>       | <span data-ttu-id="083fe-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="083fe-119">Type</span></span> | <span data-ttu-id="083fe-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="083fe-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="083fe-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="083fe-121">Authorization</span></span>  | <span data-ttu-id="083fe-122">string</span><span class="sxs-lookup"><span data-stu-id="083fe-122">string</span></span>  | <span data-ttu-id="083fe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="083fe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="083fe-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="083fe-125">Request body</span></span>
<span data-ttu-id="083fe-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="083fe-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="083fe-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="083fe-129">Property</span></span>     | <span data-ttu-id="083fe-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="083fe-130">Type</span></span>   |<span data-ttu-id="083fe-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="083fe-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="083fe-132">city</span><span class="sxs-lookup"><span data-stu-id="083fe-132">city</span></span>|<span data-ttu-id="083fe-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-133">String</span></span>||
|<span data-ttu-id="083fe-134">country</span><span class="sxs-lookup"><span data-stu-id="083fe-134">country</span></span>|<span data-ttu-id="083fe-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-135">String</span></span>||
|<span data-ttu-id="083fe-136">department</span><span class="sxs-lookup"><span data-stu-id="083fe-136">department</span></span>|<span data-ttu-id="083fe-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-137">String</span></span>||
|<span data-ttu-id="083fe-138">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="083fe-138">onPremisesSyncEnabled</span></span>|<span data-ttu-id="083fe-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="083fe-139">Boolean</span></span>||
|<span data-ttu-id="083fe-140">displayName</span><span class="sxs-lookup"><span data-stu-id="083fe-140">displayName</span></span>|<span data-ttu-id="083fe-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-141">String</span></span>||
|<span data-ttu-id="083fe-142">givenName</span><span class="sxs-lookup"><span data-stu-id="083fe-142">givenName</span></span>|<span data-ttu-id="083fe-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-143">String</span></span>||
|<span data-ttu-id="083fe-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="083fe-144">jobTitle</span></span>|<span data-ttu-id="083fe-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-145">String</span></span>||
|<span data-ttu-id="083fe-146">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="083fe-146">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="083fe-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="083fe-147">DateTimeOffset</span></span>||
|<span data-ttu-id="083fe-148">email</span><span class="sxs-lookup"><span data-stu-id="083fe-148">mail</span></span>|<span data-ttu-id="083fe-149">String</span><span class="sxs-lookup"><span data-stu-id="083fe-149">String</span></span>||
|<span data-ttu-id="083fe-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="083fe-150">mailNickname</span></span>|<span data-ttu-id="083fe-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-151">String</span></span>||
|<span data-ttu-id="083fe-152">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="083fe-152">mobilePhone</span></span>|<span data-ttu-id="083fe-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-153">String</span></span>||
|<span data-ttu-id="083fe-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="083fe-154">officeLocation</span></span>|<span data-ttu-id="083fe-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-155">String</span></span>||
|<span data-ttu-id="083fe-156">postalCode</span><span class="sxs-lookup"><span data-stu-id="083fe-156">postalCode</span></span>|<span data-ttu-id="083fe-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-157">String</span></span>||
|<span data-ttu-id="083fe-158">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="083fe-158">proxyAddresses</span></span>|<span data-ttu-id="083fe-159">String</span><span class="sxs-lookup"><span data-stu-id="083fe-159">String</span></span>||
|<span data-ttu-id="083fe-160">state</span><span class="sxs-lookup"><span data-stu-id="083fe-160">state</span></span>|<span data-ttu-id="083fe-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-161">String</span></span>||
|<span data-ttu-id="083fe-162">streetAddress</span><span class="sxs-lookup"><span data-stu-id="083fe-162">streetAddress</span></span>|<span data-ttu-id="083fe-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-163">String</span></span>||
|<span data-ttu-id="083fe-164">surname</span><span class="sxs-lookup"><span data-stu-id="083fe-164">surname</span></span>|<span data-ttu-id="083fe-165">String</span><span class="sxs-lookup"><span data-stu-id="083fe-165">String</span></span>||
|<span data-ttu-id="083fe-166">businessPhones</span><span class="sxs-lookup"><span data-stu-id="083fe-166">businessPhones</span></span>|<span data-ttu-id="083fe-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="083fe-167">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="083fe-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="083fe-168">Response</span></span>

<span data-ttu-id="083fe-169">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [orgContact](../resources/orgcontact.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="083fe-169">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="083fe-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="083fe-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="083fe-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="083fe-171">Request</span></span>
<span data-ttu-id="083fe-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="083fe-172">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="083fe-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="083fe-173">Response</span></span>
<span data-ttu-id="083fe-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="083fe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="083fe-177">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="083fe-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="083fe-178">Basic</span><span class="sxs-lookup"><span data-stu-id="083fe-178">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_orgcontact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="083fe-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="083fe-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_orgcontact-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/orgcontact-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
