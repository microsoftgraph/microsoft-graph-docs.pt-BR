---
title: Atualizar mobileAppManagementPolicy
description: Atualize as propriedades de um objeto de política de gerenciamento de aplicativo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b553a291ce986a3084403c55f3c991fb260c4828
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401642"
---
# <a name="update-mobileappmanagementpolicy"></a><span data-ttu-id="df952-103">Atualizar mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="df952-103">Update mobileAppManagementPolicy</span></span>

<span data-ttu-id="df952-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df952-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df952-105">Atualize as propriedades de [um objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df952-105">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="df952-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df952-106">Permissions</span></span>

<span data-ttu-id="df952-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df952-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df952-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df952-109">Permission type</span></span>|<span data-ttu-id="df952-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df952-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df952-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df952-111">Delegated (work or school account)</span></span>|<span data-ttu-id="df952-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="df952-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="df952-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df952-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df952-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df952-114">Not supported.</span></span>|
|<span data-ttu-id="df952-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df952-115">Application</span></span> | <span data-ttu-id="df952-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df952-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df952-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df952-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileAppManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="df952-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df952-118">Request headers</span></span>

|<span data-ttu-id="df952-119">Nome</span><span class="sxs-lookup"><span data-stu-id="df952-119">Name</span></span>|<span data-ttu-id="df952-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="df952-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="df952-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="df952-121">Authorization</span></span>|<span data-ttu-id="df952-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df952-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="df952-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df952-124">Content-Type</span></span>|<span data-ttu-id="df952-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df952-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df952-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df952-127">Request body</span></span>

<span data-ttu-id="df952-128">No corpo da solicitação, fornece uma representação JSON do [objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="df952-128">In the request body, supply a JSON representation of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

<span data-ttu-id="df952-129">No corpo da solicitação, fornece os valores para os campos listados abaixo que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="df952-129">In the request body, supply the values for fields listed below that should be updated.</span></span> <span data-ttu-id="df952-130">**Observação:** Não é possível `PATCH` usar a operação com as outras `appliesTo` propriedades.</span><span class="sxs-lookup"><span data-stu-id="df952-130">**Note:** You cannot use `PATCH` operation for `appliesTo` with the other properties.</span></span>

|<span data-ttu-id="df952-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df952-131">Property</span></span>|<span data-ttu-id="df952-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="df952-132">Type</span></span>|<span data-ttu-id="df952-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="df952-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df952-134">appliesTo</span><span class="sxs-lookup"><span data-stu-id="df952-134">appliesTo</span></span>|<span data-ttu-id="df952-135">policyScope</span><span class="sxs-lookup"><span data-stu-id="df952-135">policyScope</span></span>|<span data-ttu-id="df952-136">Determina os grupos aos quais essa configuração de política se aplica.</span><span class="sxs-lookup"><span data-stu-id="df952-136">Determines the groups this policy setting applies to.</span></span> <span data-ttu-id="df952-137">Os valores possíveis são: `none` , `all` , `selected` **Importante:** `selected` não pode ser usado ao especificar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="df952-137">Possible values are: `none`, `all`, `selected` **Important:** `selected` cannot be used when specifying this property.</span></span> <span data-ttu-id="df952-138">Use [includedGroups](../api/mobileappmanagementpolicies-post-includedgroups.md) para adicionar grupos específicos.</span><span class="sxs-lookup"><span data-stu-id="df952-138">Use [includedGroups](../api/mobileappmanagementpolicies-post-includedgroups.md) to add specific groups.</span></span>|
|<span data-ttu-id="df952-139">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="df952-139">complianceUrl</span></span>|<span data-ttu-id="df952-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df952-140">String</span></span>|<span data-ttu-id="df952-141">URL de conformidade do aplicativo de gerenciamento de mobilidade</span><span class="sxs-lookup"><span data-stu-id="df952-141">Compliance URL of the mobility management application</span></span>|
|<span data-ttu-id="df952-142">discoveryUrl</span><span class="sxs-lookup"><span data-stu-id="df952-142">discoveryUrl</span></span>|<span data-ttu-id="df952-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df952-143">String</span></span>|<span data-ttu-id="df952-144">URL de descoberta do aplicativo de gerenciamento de mobilidade</span><span class="sxs-lookup"><span data-stu-id="df952-144">Discovery URL of the mobility management application</span></span>|
|<span data-ttu-id="df952-145">termsOfUseUrl</span><span class="sxs-lookup"><span data-stu-id="df952-145">termsOfUseUrl</span></span>|<span data-ttu-id="df952-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df952-146">String</span></span>|<span data-ttu-id="df952-147">TERMOS DE USO URL do aplicativo de gerenciamento de mobilidade</span><span class="sxs-lookup"><span data-stu-id="df952-147">Terms of Use URL of the mobility management application</span></span>|

## <a name="response"></a><span data-ttu-id="df952-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="df952-148">Response</span></span>

<span data-ttu-id="df952-149">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df952-149">If successful, this method returns a `200 OK` response code and an updated [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df952-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="df952-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df952-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df952-151">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="df952-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="df952-152">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
