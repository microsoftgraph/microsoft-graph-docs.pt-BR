---
title: Atualizar deviceManagementPartner
description: Atualize as propriedades de um objeto deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: db0d71eb1bb6505034b4e66244721ce5c0dfc7c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072169"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="09920-103">Atualizar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="09920-103">Update deviceManagementPartner</span></span>

<span data-ttu-id="09920-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09920-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09920-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09920-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09920-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09920-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09920-107">Atualize as propriedades de um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="09920-107">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09920-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09920-108">Prerequisites</span></span>
<span data-ttu-id="09920-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09920-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09920-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09920-111">Permission type</span></span>|<span data-ttu-id="09920-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09920-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09920-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09920-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09920-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09920-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="09920-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09920-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09920-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09920-116">Not supported.</span></span>|
|<span data-ttu-id="09920-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09920-117">Application</span></span>|<span data-ttu-id="09920-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09920-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09920-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09920-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="09920-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09920-120">Request headers</span></span>
|<span data-ttu-id="09920-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09920-121">Header</span></span>|<span data-ttu-id="09920-122">Valor</span><span class="sxs-lookup"><span data-stu-id="09920-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09920-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="09920-123">Authorization</span></span>|<span data-ttu-id="09920-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09920-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09920-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09920-125">Accept</span></span>|<span data-ttu-id="09920-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09920-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09920-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09920-127">Request body</span></span>
<span data-ttu-id="09920-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="09920-128">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="09920-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="09920-129">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="09920-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09920-130">Property</span></span>|<span data-ttu-id="09920-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="09920-131">Type</span></span>|<span data-ttu-id="09920-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="09920-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09920-133">id</span><span class="sxs-lookup"><span data-stu-id="09920-133">id</span></span>|<span data-ttu-id="09920-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09920-134">String</span></span>|<span data-ttu-id="09920-135">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="09920-135">Id of the entity</span></span>|
|<span data-ttu-id="09920-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="09920-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="09920-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09920-137">DateTimeOffset</span></span>|<span data-ttu-id="09920-138">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="09920-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="09920-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="09920-139">partnerState</span></span>|[<span data-ttu-id="09920-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="09920-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="09920-141">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="09920-141">Partner state of this tenant.</span></span> <span data-ttu-id="09920-142">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="09920-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="09920-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="09920-143">partnerAppType</span></span>|[<span data-ttu-id="09920-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="09920-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="09920-145">Tipo de aplicativo de parceiro.</span><span class="sxs-lookup"><span data-stu-id="09920-145">Partner App type.</span></span> <span data-ttu-id="09920-146">Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="09920-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="09920-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="09920-147">singleTenantAppId</span></span>|<span data-ttu-id="09920-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09920-148">String</span></span>|<span data-ttu-id="09920-149">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="09920-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="09920-150">displayName</span><span class="sxs-lookup"><span data-stu-id="09920-150">displayName</span></span>|<span data-ttu-id="09920-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09920-151">String</span></span>|<span data-ttu-id="09920-152">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="09920-152">Partner display name</span></span>|
|<span data-ttu-id="09920-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="09920-153">isConfigured</span></span>|<span data-ttu-id="09920-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="09920-154">Boolean</span></span>|<span data-ttu-id="09920-155">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="09920-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="09920-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="09920-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="09920-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09920-157">DateTimeOffset</span></span>|<span data-ttu-id="09920-158">DateTime em UTC quando o PartnerDevices será removido.</span><span class="sxs-lookup"><span data-stu-id="09920-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="09920-159">Isso se tornará obselete em breve.</span><span class="sxs-lookup"><span data-stu-id="09920-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="09920-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="09920-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="09920-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09920-161">DateTimeOffset</span></span>|<span data-ttu-id="09920-162">DateTime em UTC quando PartnerDevices será marcado como não compatível.</span><span class="sxs-lookup"><span data-stu-id="09920-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="09920-163">Isso se tornará obselete em breve.</span><span class="sxs-lookup"><span data-stu-id="09920-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="09920-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="09920-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="09920-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09920-165">DateTimeOffset</span></span>|<span data-ttu-id="09920-166">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="09920-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="09920-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="09920-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="09920-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09920-168">DateTimeOffset</span></span>|<span data-ttu-id="09920-169">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="09920-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|
|<span data-ttu-id="09920-170">groupsRequiringPartnerEnrollment</span><span class="sxs-lookup"><span data-stu-id="09920-170">groupsRequiringPartnerEnrollment</span></span>|<span data-ttu-id="09920-171">coleção [deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="09920-171">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="09920-172">Grupos de usuários que especificam se o registro é por meio de um parceiro.</span><span class="sxs-lookup"><span data-stu-id="09920-172">User groups that specifies whether enrollment is through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="09920-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="09920-173">Response</span></span>
<span data-ttu-id="09920-174">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09920-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09920-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09920-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="09920-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09920-176">Request</span></span>
<span data-ttu-id="09920-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09920-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 1072

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="09920-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="09920-178">Response</span></span>
<span data-ttu-id="09920-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09920-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1121

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```






