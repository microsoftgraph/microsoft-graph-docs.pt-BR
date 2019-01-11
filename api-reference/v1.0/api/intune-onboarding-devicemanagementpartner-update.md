---
title: Atualizar deviceManagementPartner
description: Atualize as propriedades de um objeto deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c8e9425968d00805eb8640ff3a7e19380a92c6dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838777"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="a0528-103">Atualizar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="a0528-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="a0528-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0528-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0528-105">Atualize as propriedades de um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="a0528-105">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0528-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0528-106">Prerequisites</span></span>
<span data-ttu-id="a0528-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0528-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0528-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0528-109">Permission type</span></span>|<span data-ttu-id="a0528-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0528-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0528-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0528-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0528-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0528-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a0528-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0528-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0528-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0528-114">Not supported.</span></span>|
|<span data-ttu-id="a0528-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0528-115">Application</span></span>|<span data-ttu-id="a0528-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0528-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0528-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0528-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="a0528-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0528-118">Request headers</span></span>
|<span data-ttu-id="a0528-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0528-119">Header</span></span>|<span data-ttu-id="a0528-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a0528-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0528-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0528-121">Authorization</span></span>|<span data-ttu-id="a0528-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0528-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0528-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0528-123">Accept</span></span>|<span data-ttu-id="a0528-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a0528-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0528-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0528-125">Request body</span></span>
<span data-ttu-id="a0528-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="a0528-126">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="a0528-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="a0528-127">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="a0528-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0528-128">Property</span></span>|<span data-ttu-id="a0528-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0528-129">Type</span></span>|<span data-ttu-id="a0528-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0528-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0528-131">id</span><span class="sxs-lookup"><span data-stu-id="a0528-131">id</span></span>|<span data-ttu-id="a0528-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0528-132">String</span></span>|<span data-ttu-id="a0528-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a0528-133">Not yet documented</span></span>|
|<span data-ttu-id="a0528-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="a0528-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="a0528-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0528-135">DateTimeOffset</span></span>|<span data-ttu-id="a0528-136">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="a0528-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="a0528-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="a0528-137">partnerState</span></span>|[<span data-ttu-id="a0528-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="a0528-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="a0528-139">Estado de parceiro deste locatário.</span><span class="sxs-lookup"><span data-stu-id="a0528-139">Partner state of this tenant.</span></span> <span data-ttu-id="a0528-140">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="a0528-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="a0528-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="a0528-141">partnerAppType</span></span>|[<span data-ttu-id="a0528-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="a0528-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="a0528-143">Tipo de aplicativo de parceiro.</span><span class="sxs-lookup"><span data-stu-id="a0528-143">Partner App type.</span></span> <span data-ttu-id="a0528-144">Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="a0528-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="a0528-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="a0528-145">singleTenantAppId</span></span>|<span data-ttu-id="a0528-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0528-146">String</span></span>|<span data-ttu-id="a0528-147">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="a0528-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="a0528-148">displayName</span><span class="sxs-lookup"><span data-stu-id="a0528-148">displayName</span></span>|<span data-ttu-id="a0528-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0528-149">String</span></span>|<span data-ttu-id="a0528-150">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="a0528-150">Partner display name</span></span>|
|<span data-ttu-id="a0528-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="a0528-151">isConfigured</span></span>|<span data-ttu-id="a0528-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="a0528-152">Boolean</span></span>|<span data-ttu-id="a0528-153">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="a0528-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="a0528-154">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0528-154">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="a0528-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0528-155">DateTimeOffset</span></span>|<span data-ttu-id="a0528-156">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="a0528-156">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="a0528-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="a0528-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="a0528-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0528-158">DateTimeOffset</span></span>|<span data-ttu-id="a0528-159">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="a0528-159">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="a0528-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0528-160">Response</span></span>
<span data-ttu-id="a0528-161">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0528-161">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0528-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0528-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="a0528-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0528-163">Request</span></span>
<span data-ttu-id="a0528-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0528-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0528-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0528-165">Response</span></span>
<span data-ttu-id="a0528-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0528-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



