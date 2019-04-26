---
title: Atualizar deviceManagementPartner
description: Atualize as propriedades de um objeto deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb90210e753becbee984cc9c809e3cbdee089bee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561513"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="e1216-103">Atualizar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="e1216-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="e1216-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1216-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1216-105">Atualize as propriedades de um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e1216-105">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1216-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1216-106">Prerequisites</span></span>
<span data-ttu-id="e1216-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1216-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1216-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1216-109">Permission type</span></span>|<span data-ttu-id="e1216-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1216-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1216-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1216-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1216-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1216-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e1216-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1216-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1216-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1216-114">Not supported.</span></span>|
|<span data-ttu-id="e1216-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1216-115">Application</span></span>|<span data-ttu-id="e1216-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1216-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1216-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1216-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="e1216-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1216-118">Request headers</span></span>
|<span data-ttu-id="e1216-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1216-119">Header</span></span>|<span data-ttu-id="e1216-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e1216-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1216-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1216-121">Authorization</span></span>|<span data-ttu-id="e1216-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1216-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1216-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1216-123">Accept</span></span>|<span data-ttu-id="e1216-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e1216-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1216-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1216-125">Request body</span></span>
<span data-ttu-id="e1216-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e1216-126">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="e1216-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e1216-127">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="e1216-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1216-128">Property</span></span>|<span data-ttu-id="e1216-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1216-129">Type</span></span>|<span data-ttu-id="e1216-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1216-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1216-131">id</span><span class="sxs-lookup"><span data-stu-id="e1216-131">id</span></span>|<span data-ttu-id="e1216-132">String</span><span class="sxs-lookup"><span data-stu-id="e1216-132">String</span></span>|<span data-ttu-id="e1216-133">ID da entidade</span><span class="sxs-lookup"><span data-stu-id="e1216-133">Id of the entity</span></span>|
|<span data-ttu-id="e1216-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="e1216-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="e1216-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1216-135">DateTimeOffset</span></span>|<span data-ttu-id="e1216-136">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="e1216-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="e1216-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="e1216-137">partnerState</span></span>|[<span data-ttu-id="e1216-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="e1216-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="e1216-139">Estado do parceiro desse locatário.</span><span class="sxs-lookup"><span data-stu-id="e1216-139">Partner state of this tenant.</span></span> <span data-ttu-id="e1216-140">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="e1216-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="e1216-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="e1216-141">partnerAppType</span></span>|[<span data-ttu-id="e1216-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="e1216-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="e1216-143">Tipo de aplicativo de parceiro.</span><span class="sxs-lookup"><span data-stu-id="e1216-143">Partner App type.</span></span> <span data-ttu-id="e1216-144">Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="e1216-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="e1216-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="e1216-145">singleTenantAppId</span></span>|<span data-ttu-id="e1216-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1216-146">String</span></span>|<span data-ttu-id="e1216-147">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="e1216-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="e1216-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e1216-148">displayName</span></span>|<span data-ttu-id="e1216-149">String</span><span class="sxs-lookup"><span data-stu-id="e1216-149">String</span></span>|<span data-ttu-id="e1216-150">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="e1216-150">Partner display name</span></span>|
|<span data-ttu-id="e1216-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="e1216-151">isConfigured</span></span>|<span data-ttu-id="e1216-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1216-152">Boolean</span></span>|<span data-ttu-id="e1216-153">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="e1216-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="e1216-154">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1216-154">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="e1216-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1216-155">DateTimeOffset</span></span>|<span data-ttu-id="e1216-156">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="e1216-156">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="e1216-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="e1216-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="e1216-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1216-158">DateTimeOffset</span></span>|<span data-ttu-id="e1216-159">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="e1216-159">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="e1216-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1216-160">Response</span></span>
<span data-ttu-id="e1216-161">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1216-161">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1216-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1216-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1216-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1216-163">Request</span></span>
<span data-ttu-id="e1216-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1216-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e1216-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1216-165">Response</span></span>
<span data-ttu-id="e1216-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1216-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```



