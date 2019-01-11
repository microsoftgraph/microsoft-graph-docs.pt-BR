---
title: Atualizar deviceManagementPartner
description: Atualize as propriedades de um objeto deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 83ba5bf2e022b6961182a8f8c1ac17dec79ed959
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843152"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="0c055-103">Atualizar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="0c055-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="0c055-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0c055-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c055-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0c055-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c055-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0c055-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c055-107">Atualize as propriedades de um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="0c055-107">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c055-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c055-108">Prerequisites</span></span>
<span data-ttu-id="0c055-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c055-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c055-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c055-111">Permission type</span></span>|<span data-ttu-id="0c055-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c055-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c055-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c055-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c055-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c055-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0c055-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c055-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c055-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c055-116">Not supported.</span></span>|
|<span data-ttu-id="0c055-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c055-117">Application</span></span>|<span data-ttu-id="0c055-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c055-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c055-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c055-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="0c055-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c055-120">Request headers</span></span>
|<span data-ttu-id="0c055-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c055-121">Header</span></span>|<span data-ttu-id="0c055-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0c055-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c055-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c055-123">Authorization</span></span>|<span data-ttu-id="0c055-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c055-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c055-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c055-125">Accept</span></span>|<span data-ttu-id="0c055-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c055-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c055-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c055-127">Request body</span></span>
<span data-ttu-id="0c055-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="0c055-128">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="0c055-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="0c055-129">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="0c055-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c055-130">Property</span></span>|<span data-ttu-id="0c055-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c055-131">Type</span></span>|<span data-ttu-id="0c055-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c055-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c055-133">id</span><span class="sxs-lookup"><span data-stu-id="0c055-133">id</span></span>|<span data-ttu-id="0c055-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c055-134">String</span></span>|<span data-ttu-id="0c055-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0c055-135">Not yet documented</span></span>|
|<span data-ttu-id="0c055-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="0c055-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="0c055-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c055-137">DateTimeOffset</span></span>|<span data-ttu-id="0c055-138">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="0c055-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="0c055-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="0c055-139">partnerState</span></span>|[<span data-ttu-id="0c055-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="0c055-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="0c055-141">Estado de parceiro deste locatário.</span><span class="sxs-lookup"><span data-stu-id="0c055-141">Partner state of this tenant.</span></span> <span data-ttu-id="0c055-142">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="0c055-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="0c055-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="0c055-143">partnerAppType</span></span>|[<span data-ttu-id="0c055-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="0c055-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="0c055-145">Tipo de aplicativo de parceiro.</span><span class="sxs-lookup"><span data-stu-id="0c055-145">Partner App type.</span></span> <span data-ttu-id="0c055-146">Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="0c055-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="0c055-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="0c055-147">singleTenantAppId</span></span>|<span data-ttu-id="0c055-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c055-148">String</span></span>|<span data-ttu-id="0c055-149">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="0c055-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="0c055-150">displayName</span><span class="sxs-lookup"><span data-stu-id="0c055-150">displayName</span></span>|<span data-ttu-id="0c055-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c055-151">String</span></span>|<span data-ttu-id="0c055-152">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="0c055-152">Partner display name</span></span>|
|<span data-ttu-id="0c055-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="0c055-153">isConfigured</span></span>|<span data-ttu-id="0c055-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="0c055-154">Boolean</span></span>|<span data-ttu-id="0c055-155">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="0c055-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="0c055-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="0c055-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="0c055-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c055-157">DateTimeOffset</span></span>|<span data-ttu-id="0c055-158">Data e hora em UTC quando PartnerDevices serão removidas.</span><span class="sxs-lookup"><span data-stu-id="0c055-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="0c055-159">Isso tornará obsoleto em breve.</span><span class="sxs-lookup"><span data-stu-id="0c055-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="0c055-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="0c055-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="0c055-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c055-161">DateTimeOffset</span></span>|<span data-ttu-id="0c055-162">Data e hora em UTC quando PartnerDevices será marcada como incompatível.</span><span class="sxs-lookup"><span data-stu-id="0c055-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="0c055-163">Isso tornará obsoleto em breve.</span><span class="sxs-lookup"><span data-stu-id="0c055-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="0c055-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c055-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="0c055-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c055-165">DateTimeOffset</span></span>|<span data-ttu-id="0c055-166">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="0c055-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="0c055-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="0c055-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="0c055-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c055-168">DateTimeOffset</span></span>|<span data-ttu-id="0c055-169">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="0c055-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="0c055-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c055-170">Response</span></span>
<span data-ttu-id="0c055-171">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c055-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c055-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c055-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c055-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c055-173">Request</span></span>
<span data-ttu-id="0c055-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c055-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 602

{
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

### <a name="response"></a><span data-ttu-id="0c055-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c055-175">Response</span></span>
<span data-ttu-id="0c055-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c055-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





