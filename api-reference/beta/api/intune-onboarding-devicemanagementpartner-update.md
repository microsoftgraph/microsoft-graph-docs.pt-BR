---
title: Atualizar deviceManagementPartner
description: Atualize as propriedades de um objeto deviceManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bff6eec75e1c29e219cd8f2761c6b270a458728d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900030"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="5de3e-103">Atualizar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="5de3e-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="5de3e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5de3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5de3e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5de3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5de3e-106">Atualize as propriedades de um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="5de3e-106">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5de3e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5de3e-107">Prerequisites</span></span>
<span data-ttu-id="5de3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5de3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5de3e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5de3e-110">Permission type</span></span>|<span data-ttu-id="5de3e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5de3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5de3e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5de3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5de3e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de3e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5de3e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5de3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5de3e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5de3e-115">Not supported.</span></span>|
|<span data-ttu-id="5de3e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5de3e-116">Application</span></span>|<span data-ttu-id="5de3e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5de3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5de3e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5de3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="5de3e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5de3e-119">Request headers</span></span>
|<span data-ttu-id="5de3e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5de3e-120">Header</span></span>|<span data-ttu-id="5de3e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5de3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5de3e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5de3e-122">Authorization</span></span>|<span data-ttu-id="5de3e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5de3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5de3e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5de3e-124">Accept</span></span>|<span data-ttu-id="5de3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5de3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5de3e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5de3e-126">Request body</span></span>
<span data-ttu-id="5de3e-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="5de3e-127">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="5de3e-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="5de3e-128">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="5de3e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5de3e-129">Property</span></span>|<span data-ttu-id="5de3e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5de3e-130">Type</span></span>|<span data-ttu-id="5de3e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5de3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5de3e-132">id</span><span class="sxs-lookup"><span data-stu-id="5de3e-132">id</span></span>|<span data-ttu-id="5de3e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5de3e-133">String</span></span>|<span data-ttu-id="5de3e-134">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="5de3e-134">Id of the entity</span></span>|
|<span data-ttu-id="5de3e-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="5de3e-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="5de3e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5de3e-136">DateTimeOffset</span></span>|<span data-ttu-id="5de3e-137">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5de3e-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="5de3e-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="5de3e-138">partnerState</span></span>|[<span data-ttu-id="5de3e-139">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="5de3e-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="5de3e-140">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="5de3e-140">Partner state of this tenant.</span></span> <span data-ttu-id="5de3e-141">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="5de3e-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="5de3e-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="5de3e-142">partnerAppType</span></span>|[<span data-ttu-id="5de3e-143">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="5de3e-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="5de3e-144">Tipo de aplicativo de parceiro.</span><span class="sxs-lookup"><span data-stu-id="5de3e-144">Partner App type.</span></span> <span data-ttu-id="5de3e-145">Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="5de3e-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="5de3e-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="5de3e-146">singleTenantAppId</span></span>|<span data-ttu-id="5de3e-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5de3e-147">String</span></span>|<span data-ttu-id="5de3e-148">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="5de3e-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="5de3e-149">displayName</span><span class="sxs-lookup"><span data-stu-id="5de3e-149">displayName</span></span>|<span data-ttu-id="5de3e-150">String</span><span class="sxs-lookup"><span data-stu-id="5de3e-150">String</span></span>|<span data-ttu-id="5de3e-151">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="5de3e-151">Partner display name</span></span>|
|<span data-ttu-id="5de3e-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="5de3e-152">isConfigured</span></span>|<span data-ttu-id="5de3e-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="5de3e-153">Boolean</span></span>|<span data-ttu-id="5de3e-154">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="5de3e-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="5de3e-155">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="5de3e-155">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="5de3e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5de3e-156">DateTimeOffset</span></span>|<span data-ttu-id="5de3e-157">DateTime em UTC quando o PartnerDevices será removido.</span><span class="sxs-lookup"><span data-stu-id="5de3e-157">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="5de3e-158">Isso se tornará obselete em breve.</span><span class="sxs-lookup"><span data-stu-id="5de3e-158">This will become obselete soon.</span></span>|
|<span data-ttu-id="5de3e-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="5de3e-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="5de3e-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5de3e-160">DateTimeOffset</span></span>|<span data-ttu-id="5de3e-161">DateTime em UTC quando PartnerDevices será marcado como não compatível.</span><span class="sxs-lookup"><span data-stu-id="5de3e-161">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="5de3e-162">Isso se tornará obselete em breve.</span><span class="sxs-lookup"><span data-stu-id="5de3e-162">This will become obselete soon.</span></span>|
|<span data-ttu-id="5de3e-163">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="5de3e-163">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="5de3e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5de3e-164">DateTimeOffset</span></span>|<span data-ttu-id="5de3e-165">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="5de3e-165">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="5de3e-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="5de3e-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="5de3e-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5de3e-167">DateTimeOffset</span></span>|<span data-ttu-id="5de3e-168">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="5de3e-168">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="5de3e-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="5de3e-169">Response</span></span>
<span data-ttu-id="5de3e-170">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5de3e-170">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5de3e-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5de3e-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="5de3e-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5de3e-172">Request</span></span>
<span data-ttu-id="5de3e-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5de3e-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 664

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
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="5de3e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="5de3e-174">Response</span></span>
<span data-ttu-id="5de3e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5de3e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 713

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
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```




