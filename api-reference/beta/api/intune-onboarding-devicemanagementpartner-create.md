---
title: Criar deviceManagementPartner
description: Criar um novo objeto deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 54851dee4415d97a6f430ef6ffaa361b5d16d2de
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791823"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="77160-103">Criar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="77160-103">Create deviceManagementPartner</span></span>

<span data-ttu-id="77160-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77160-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77160-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77160-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77160-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77160-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77160-107">Criar um novo objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="77160-107">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77160-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77160-108">Prerequisites</span></span>
<span data-ttu-id="77160-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="77160-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="77160-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77160-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77160-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77160-111">Permission type</span></span>|<span data-ttu-id="77160-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77160-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77160-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77160-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77160-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77160-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="77160-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77160-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77160-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77160-116">Not supported.</span></span>|
|<span data-ttu-id="77160-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77160-117">Application</span></span>|<span data-ttu-id="77160-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77160-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77160-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77160-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="77160-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77160-120">Request headers</span></span>
|<span data-ttu-id="77160-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77160-121">Header</span></span>|<span data-ttu-id="77160-122">Valor</span><span class="sxs-lookup"><span data-stu-id="77160-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77160-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="77160-123">Authorization</span></span>|<span data-ttu-id="77160-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77160-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77160-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77160-125">Accept</span></span>|<span data-ttu-id="77160-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77160-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77160-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77160-127">Request body</span></span>
<span data-ttu-id="77160-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="77160-128">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="77160-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="77160-129">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="77160-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77160-130">Property</span></span>|<span data-ttu-id="77160-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="77160-131">Type</span></span>|<span data-ttu-id="77160-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="77160-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77160-133">id</span><span class="sxs-lookup"><span data-stu-id="77160-133">id</span></span>|<span data-ttu-id="77160-134">String</span><span class="sxs-lookup"><span data-stu-id="77160-134">String</span></span>|<span data-ttu-id="77160-135">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="77160-135">Id of the entity</span></span>|
|<span data-ttu-id="77160-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="77160-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="77160-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77160-137">DateTimeOffset</span></span>|<span data-ttu-id="77160-138">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="77160-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="77160-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="77160-139">partnerState</span></span>|[<span data-ttu-id="77160-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="77160-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="77160-141">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="77160-141">Partner state of this tenant.</span></span> <span data-ttu-id="77160-142">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="77160-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="77160-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="77160-143">partnerAppType</span></span>|[<span data-ttu-id="77160-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="77160-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="77160-145">Tipo de aplicativo de parceiro.</span><span class="sxs-lookup"><span data-stu-id="77160-145">Partner App type.</span></span> <span data-ttu-id="77160-146">Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="77160-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="77160-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="77160-147">singleTenantAppId</span></span>|<span data-ttu-id="77160-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77160-148">String</span></span>|<span data-ttu-id="77160-149">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="77160-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="77160-150">displayName</span><span class="sxs-lookup"><span data-stu-id="77160-150">displayName</span></span>|<span data-ttu-id="77160-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77160-151">String</span></span>|<span data-ttu-id="77160-152">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="77160-152">Partner display name</span></span>|
|<span data-ttu-id="77160-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="77160-153">isConfigured</span></span>|<span data-ttu-id="77160-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="77160-154">Boolean</span></span>|<span data-ttu-id="77160-155">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="77160-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="77160-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="77160-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="77160-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77160-157">DateTimeOffset</span></span>|<span data-ttu-id="77160-158">DateTime em UTC quando o PartnerDevices será removido.</span><span class="sxs-lookup"><span data-stu-id="77160-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="77160-159">Isso se tornará obselete em breve.</span><span class="sxs-lookup"><span data-stu-id="77160-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="77160-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="77160-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="77160-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77160-161">DateTimeOffset</span></span>|<span data-ttu-id="77160-162">DateTime em UTC quando PartnerDevices será marcado como não compatível.</span><span class="sxs-lookup"><span data-stu-id="77160-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="77160-163">Isso se tornará obselete em breve.</span><span class="sxs-lookup"><span data-stu-id="77160-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="77160-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="77160-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="77160-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77160-165">DateTimeOffset</span></span>|<span data-ttu-id="77160-166">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="77160-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="77160-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="77160-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="77160-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77160-168">DateTimeOffset</span></span>|<span data-ttu-id="77160-169">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="77160-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|
|<span data-ttu-id="77160-170">groupsRequiringPartnerEnrollment</span><span class="sxs-lookup"><span data-stu-id="77160-170">groupsRequiringPartnerEnrollment</span></span>|<span data-ttu-id="77160-171">coleção [deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="77160-171">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="77160-172">Grupos de usuários que especificam se o registro é por meio de um parceiro.</span><span class="sxs-lookup"><span data-stu-id="77160-172">User groups that specifies whether enrollment is through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="77160-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="77160-173">Response</span></span>
<span data-ttu-id="77160-174">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77160-174">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77160-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77160-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="77160-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77160-176">Request</span></span>
<span data-ttu-id="77160-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77160-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
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

### <a name="response"></a><span data-ttu-id="77160-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="77160-178">Response</span></span>
<span data-ttu-id="77160-179">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="77160-179">Here is an example of the response.</span></span> <span data-ttu-id="77160-180">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="77160-180">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="77160-181">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="77160-181">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



