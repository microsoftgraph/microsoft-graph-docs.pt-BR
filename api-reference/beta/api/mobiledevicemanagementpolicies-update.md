---
title: Atualizar mobileDeviceManagementPolicy
description: Atualize as propriedades de um objeto de gerenciamento de dispositivo móvel.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ef94012247c011026b8c24a9219aa2d7c3228131
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401353"
---
# <a name="update-mobiledevicemanagementpolicy"></a><span data-ttu-id="daeca-103">Atualizar mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="daeca-103">Update mobileDeviceManagementPolicy</span></span>

<span data-ttu-id="daeca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daeca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daeca-105">Atualize as propriedades de [um objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="daeca-105">Update the properties of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="daeca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="daeca-106">Permissions</span></span>

<span data-ttu-id="daeca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daeca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daeca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="daeca-109">Permission type</span></span>|<span data-ttu-id="daeca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="daeca-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daeca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="daeca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="daeca-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="daeca-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="daeca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="daeca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daeca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daeca-114">Not supported.</span></span>|
|<span data-ttu-id="daeca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="daeca-115">Application</span></span> | <span data-ttu-id="daeca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daeca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="daeca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="daeca-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="daeca-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="daeca-118">Request headers</span></span>

|<span data-ttu-id="daeca-119">Nome</span><span class="sxs-lookup"><span data-stu-id="daeca-119">Name</span></span>|<span data-ttu-id="daeca-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="daeca-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="daeca-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="daeca-121">Authorization</span></span>|<span data-ttu-id="daeca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="daeca-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="daeca-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="daeca-124">Content-Type</span></span>|<span data-ttu-id="daeca-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="daeca-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="daeca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="daeca-127">Request body</span></span>

<span data-ttu-id="daeca-128">No corpo da solicitação, fornece uma representação JSON do [objeto mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="daeca-128">In the request body, supply a JSON representation of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

<span data-ttu-id="daeca-129">No corpo da solicitação, fornece os valores para os campos listados abaixo que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="daeca-129">In the request body, supply the values for fields listed below that should be updated.</span></span> <span data-ttu-id="daeca-130">**Observação:** Não é possível `PATCH` usar a operação com as outras `appliesTo` propriedades.</span><span class="sxs-lookup"><span data-stu-id="daeca-130">**Note:** You cannot use `PATCH` operation for `appliesTo` with the other properties.</span></span>

|<span data-ttu-id="daeca-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="daeca-131">Property</span></span>|<span data-ttu-id="daeca-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="daeca-132">Type</span></span>|<span data-ttu-id="daeca-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="daeca-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daeca-134">appliesTo</span><span class="sxs-lookup"><span data-stu-id="daeca-134">appliesTo</span></span>|<span data-ttu-id="daeca-135">policyScope</span><span class="sxs-lookup"><span data-stu-id="daeca-135">policyScope</span></span>|<span data-ttu-id="daeca-136">Determina os grupos aos quais essa configuração de política se aplica.</span><span class="sxs-lookup"><span data-stu-id="daeca-136">Determines the groups this policy setting applies to.</span></span> <span data-ttu-id="daeca-137">Os valores possíveis são: `none` , `all` , `selected` **Importante:** `selected` não pode ser usado ao especificar essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="daeca-137">Possible values are: `none`, `all`, `selected` **Important:** `selected` cannot be used when specifying this property.</span></span> <span data-ttu-id="daeca-138">Use [includedGroups](../api/mobiledevicemanagementpolicies-post-includedgroups.md) para adicionar grupos específicos.</span><span class="sxs-lookup"><span data-stu-id="daeca-138">Use [includedGroups](../api/mobiledevicemanagementpolicies-post-includedgroups.md) to add specific groups.</span></span> <span data-ttu-id="daeca-139">O `all` uso removerá todos os grupos existentes.</span><span class="sxs-lookup"><span data-stu-id="daeca-139">Using `all` will remove any existing groups.</span></span>|
|<span data-ttu-id="daeca-140">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="daeca-140">complianceUrl</span></span>|<span data-ttu-id="daeca-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="daeca-141">String</span></span>|<span data-ttu-id="daeca-142">URL de conformidade do aplicativo de gerenciamento de mobilidade</span><span class="sxs-lookup"><span data-stu-id="daeca-142">Compliance URL of the mobility management application</span></span>|
|<span data-ttu-id="daeca-143">discoveryUrl</span><span class="sxs-lookup"><span data-stu-id="daeca-143">discoveryUrl</span></span>|<span data-ttu-id="daeca-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="daeca-144">String</span></span>|<span data-ttu-id="daeca-145">URL de descoberta do aplicativo de gerenciamento de mobilidade</span><span class="sxs-lookup"><span data-stu-id="daeca-145">Discovery URL of the mobility management application</span></span>|
|<span data-ttu-id="daeca-146">termsOfUseUrl</span><span class="sxs-lookup"><span data-stu-id="daeca-146">termsOfUseUrl</span></span>|<span data-ttu-id="daeca-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="daeca-147">String</span></span>|<span data-ttu-id="daeca-148">TERMOS DE USO URL do aplicativo de gerenciamento de mobilidade</span><span class="sxs-lookup"><span data-stu-id="daeca-148">Terms of Use URL of the mobility management application</span></span>|

## <a name="response"></a><span data-ttu-id="daeca-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="daeca-149">Response</span></span>

<span data-ttu-id="daeca-150">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="daeca-150">If successful, this method returns a `200 OK` response code and an updated [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="daeca-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="daeca-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="daeca-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="daeca-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mobilitymanagementpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "complianceUrl": "https://portal.uem.contoso.com/?portalAction=Compliance",
  "discoveryUrl": "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc",
  "termsOfUseUrl": "https://portal.uem.contoso.com/TermsofUse.aspx"
}
```

### <a name="response"></a><span data-ttu-id="daeca-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="daeca-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
