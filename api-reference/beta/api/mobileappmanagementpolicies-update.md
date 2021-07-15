---
title: Atualizar mobileAppManagementPolicy
description: Atualize as propriedades de um objeto de política de gerenciamento de aplicativo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fe577a8c27b7c32e320416da74a4fa34fabb3339
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440341"
---
# <a name="update-mobileappmanagementpolicy"></a><span data-ttu-id="16ed6-103">Atualizar mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="16ed6-103">Update mobileAppManagementPolicy</span></span>

<span data-ttu-id="16ed6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16ed6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16ed6-105">Atualize as propriedades de [um objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="16ed6-105">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="16ed6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="16ed6-106">Permissions</span></span>

<span data-ttu-id="16ed6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16ed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16ed6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16ed6-109">Permission type</span></span>|<span data-ttu-id="16ed6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16ed6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16ed6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16ed6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16ed6-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="16ed6-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="16ed6-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16ed6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16ed6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16ed6-114">Not supported.</span></span>|
|<span data-ttu-id="16ed6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16ed6-115">Application</span></span> | <span data-ttu-id="16ed6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16ed6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16ed6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16ed6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileAppManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="16ed6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16ed6-118">Request headers</span></span>

|<span data-ttu-id="16ed6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="16ed6-119">Name</span></span>|<span data-ttu-id="16ed6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="16ed6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="16ed6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="16ed6-121">Authorization</span></span>|<span data-ttu-id="16ed6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16ed6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="16ed6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16ed6-124">Content-Type</span></span>|<span data-ttu-id="16ed6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16ed6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16ed6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16ed6-127">Request body</span></span>

<span data-ttu-id="16ed6-128">No corpo da solicitação, fornece uma representação JSON do [objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="16ed6-128">In the request body, supply a JSON representation of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

<span data-ttu-id="16ed6-129">No corpo da solicitação, fornece os valores para os campos listados abaixo que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="16ed6-129">In the request body, supply the values for fields listed below that should be updated.</span></span> <span data-ttu-id="16ed6-130">**Observação:** Não é possível `PATCH` usar a operação com as outras `appliesTo` propriedades.</span><span class="sxs-lookup"><span data-stu-id="16ed6-130">**Note:** You cannot use `PATCH` operation for `appliesTo` with the other properties.</span></span>

|<span data-ttu-id="16ed6-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16ed6-131">Property</span></span>|<span data-ttu-id="16ed6-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="16ed6-132">Type</span></span>|<span data-ttu-id="16ed6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="16ed6-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16ed6-134">appliesTo</span><span class="sxs-lookup"><span data-stu-id="16ed6-134">appliesTo</span></span>|<span data-ttu-id="16ed6-135">policyScope</span><span class="sxs-lookup"><span data-stu-id="16ed6-135">policyScope</span></span>|<span data-ttu-id="16ed6-136">Determina os grupos aos quais essa configuração de política se aplica.</span><span class="sxs-lookup"><span data-stu-id="16ed6-136">Determines the groups this policy setting applies to.</span></span> <span data-ttu-id="16ed6-137">Os valores possíveis são: `none` , `all` , `selected` **Importante:** `selected` não pode ser usado ao especificar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="16ed6-137">Possible values are: `none`, `all`, `selected` **Important:** `selected` cannot be used when specifying this property.</span></span> <span data-ttu-id="16ed6-138">Use [includedGroups](../api/mobileappmanagementpolicies-post-includedgroups.md) para adicionar grupos específicos.</span><span class="sxs-lookup"><span data-stu-id="16ed6-138">Use [includedGroups](../api/mobileappmanagementpolicies-post-includedgroups.md) to add specific groups.</span></span>|
|<span data-ttu-id="16ed6-139">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="16ed6-139">complianceUrl</span></span>|<span data-ttu-id="16ed6-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16ed6-140">String</span></span>|<span data-ttu-id="16ed6-141">URL de conformidade do aplicativo de gerenciamento de mobilidade</span><span class="sxs-lookup"><span data-stu-id="16ed6-141">Compliance URL of the mobility management application</span></span>|
|<span data-ttu-id="16ed6-142">discoveryUrl</span><span class="sxs-lookup"><span data-stu-id="16ed6-142">discoveryUrl</span></span>|<span data-ttu-id="16ed6-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16ed6-143">String</span></span>|<span data-ttu-id="16ed6-144">URL de descoberta do aplicativo de gerenciamento de mobilidade</span><span class="sxs-lookup"><span data-stu-id="16ed6-144">Discovery URL of the mobility management application</span></span>|
|<span data-ttu-id="16ed6-145">termsOfUseUrl</span><span class="sxs-lookup"><span data-stu-id="16ed6-145">termsOfUseUrl</span></span>|<span data-ttu-id="16ed6-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16ed6-146">String</span></span>|<span data-ttu-id="16ed6-147">TERMOS DE USO URL do aplicativo de gerenciamento de mobilidade</span><span class="sxs-lookup"><span data-stu-id="16ed6-147">Terms of Use URL of the mobility management application</span></span>|

## <a name="response"></a><span data-ttu-id="16ed6-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="16ed6-148">Response</span></span>

<span data-ttu-id="16ed6-149">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16ed6-149">If successful, this method returns a `200 OK` response code and an updated [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16ed6-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="16ed6-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16ed6-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16ed6-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="16ed6-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="16ed6-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mobilitymanagementpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "complianceUrl": "https://portal.mg.contoso.com/?portalAction=Compliance",
  "discoveryUrl": "https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc",
  "termsOfUseUrl": "https://portal.mg.contoso.com/TermsofUse.aspx"
}
```
# <a name="c"></a>[<span data-ttu-id="16ed6-153">C#</span><span class="sxs-lookup"><span data-stu-id="16ed6-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mobilitymanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16ed6-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16ed6-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mobilitymanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16ed6-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16ed6-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mobilitymanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16ed6-156">Java</span><span class="sxs-lookup"><span data-stu-id="16ed6-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mobilitymanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="16ed6-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="16ed6-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
