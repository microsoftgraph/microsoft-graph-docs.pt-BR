---
title: Criar deviceManagementPartner
description: Criar um novo objeto deviceManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c260054415faab61efee551fb65386c18695d2b0
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086638"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="574d6-103">Criar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="574d6-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="574d6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="574d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="574d6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="574d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="574d6-106">Criar um novo objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="574d6-106">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="574d6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="574d6-107">Prerequisites</span></span>
<span data-ttu-id="574d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="574d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="574d6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="574d6-110">Permission type</span></span>|<span data-ttu-id="574d6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="574d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="574d6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="574d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="574d6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="574d6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="574d6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="574d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="574d6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="574d6-115">Not supported.</span></span>|
|<span data-ttu-id="574d6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="574d6-116">Application</span></span>|<span data-ttu-id="574d6-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="574d6-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="574d6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="574d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="574d6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="574d6-119">Request headers</span></span>
|<span data-ttu-id="574d6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="574d6-120">Header</span></span>|<span data-ttu-id="574d6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="574d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="574d6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="574d6-122">Authorization</span></span>|<span data-ttu-id="574d6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="574d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="574d6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="574d6-124">Accept</span></span>|<span data-ttu-id="574d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="574d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="574d6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="574d6-126">Request body</span></span>
<span data-ttu-id="574d6-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="574d6-127">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="574d6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="574d6-128">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="574d6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="574d6-129">Property</span></span>|<span data-ttu-id="574d6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="574d6-130">Type</span></span>|<span data-ttu-id="574d6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="574d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="574d6-132">id</span><span class="sxs-lookup"><span data-stu-id="574d6-132">id</span></span>|<span data-ttu-id="574d6-133">String</span><span class="sxs-lookup"><span data-stu-id="574d6-133">String</span></span>|<span data-ttu-id="574d6-134">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="574d6-134">Id of the entity</span></span>|
|<span data-ttu-id="574d6-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="574d6-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="574d6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="574d6-136">DateTimeOffset</span></span>|<span data-ttu-id="574d6-137">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="574d6-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="574d6-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="574d6-138">partnerState</span></span>|[<span data-ttu-id="574d6-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="574d6-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="574d6-140">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="574d6-140">Partner state of this tenant.</span></span> <span data-ttu-id="574d6-141">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="574d6-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="574d6-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="574d6-142">partnerAppType</span></span>|[<span data-ttu-id="574d6-143">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="574d6-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="574d6-144">Tipo de aplicativo de parceiro.</span><span class="sxs-lookup"><span data-stu-id="574d6-144">Partner App type.</span></span> <span data-ttu-id="574d6-145">Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="574d6-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="574d6-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="574d6-146">singleTenantAppId</span></span>|<span data-ttu-id="574d6-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="574d6-147">String</span></span>|<span data-ttu-id="574d6-148">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="574d6-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="574d6-149">displayName</span><span class="sxs-lookup"><span data-stu-id="574d6-149">displayName</span></span>|<span data-ttu-id="574d6-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="574d6-150">String</span></span>|<span data-ttu-id="574d6-151">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="574d6-151">Partner display name</span></span>|
|<span data-ttu-id="574d6-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="574d6-152">isConfigured</span></span>|<span data-ttu-id="574d6-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="574d6-153">Boolean</span></span>|<span data-ttu-id="574d6-154">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="574d6-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="574d6-155">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="574d6-155">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="574d6-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="574d6-156">DateTimeOffset</span></span>|<span data-ttu-id="574d6-157">DateTime em UTC quando o PartnerDevices será removido.</span><span class="sxs-lookup"><span data-stu-id="574d6-157">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="574d6-158">Isso se tornará obselete em breve.</span><span class="sxs-lookup"><span data-stu-id="574d6-158">This will become obselete soon.</span></span>|
|<span data-ttu-id="574d6-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="574d6-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="574d6-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="574d6-160">DateTimeOffset</span></span>|<span data-ttu-id="574d6-161">DateTime em UTC quando PartnerDevices será marcado como não compatível.</span><span class="sxs-lookup"><span data-stu-id="574d6-161">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="574d6-162">Isso se tornará obselete em breve.</span><span class="sxs-lookup"><span data-stu-id="574d6-162">This will become obselete soon.</span></span>|
|<span data-ttu-id="574d6-163">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="574d6-163">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="574d6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="574d6-164">DateTimeOffset</span></span>|<span data-ttu-id="574d6-165">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="574d6-165">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="574d6-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="574d6-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="574d6-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="574d6-167">DateTimeOffset</span></span>|<span data-ttu-id="574d6-168">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="574d6-168">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|
|<span data-ttu-id="574d6-169">groupsRequiringPartnerEnrollment</span><span class="sxs-lookup"><span data-stu-id="574d6-169">groupsRequiringPartnerEnrollment</span></span>|<span data-ttu-id="574d6-170">coleção [deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="574d6-170">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="574d6-171">Grupos de usuários que especificam se o registro é por meio de um parceiro.</span><span class="sxs-lookup"><span data-stu-id="574d6-171">User groups that specifies whether enrollment is through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="574d6-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="574d6-172">Response</span></span>
<span data-ttu-id="574d6-173">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="574d6-173">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="574d6-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="574d6-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="574d6-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="574d6-175">Request</span></span>
<span data-ttu-id="574d6-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="574d6-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
Content-type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="574d6-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="574d6-177">Response</span></span>
<span data-ttu-id="574d6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="574d6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 946

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```






