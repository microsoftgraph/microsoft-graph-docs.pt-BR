---
title: Atualizar deviceManagementPartner
description: Atualize as propriedades de um objeto deviceManagementPartner.
ms.openlocfilehash: 06dd0099657dd9b697027637c2b5388c1c8b12be
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035979"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="c6c7c-103">Atualizar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="c6c7c-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="c6c7c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6c7c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6c7c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6c7c-107">Atualize as propriedades de um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="c6c7c-107">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6c7c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6c7c-108">Prerequisites</span></span>
<span data-ttu-id="c6c7c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6c7c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6c7c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6c7c-111">Permission type</span></span>|<span data-ttu-id="c6c7c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c6c7c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6c7c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6c7c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6c7c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6c7c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c6c7c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6c7c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6c7c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-116">Not supported.</span></span>|
|<span data-ttu-id="c6c7c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6c7c-117">Application</span></span>|<span data-ttu-id="c6c7c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6c7c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6c7c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="c6c7c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c7c-120">Request headers</span></span>
|<span data-ttu-id="c6c7c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6c7c-121">Header</span></span>|<span data-ttu-id="c6c7c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c6c7c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6c7c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6c7c-123">Authorization</span></span>|<span data-ttu-id="c6c7c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6c7c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c6c7c-125">Accept</span></span>|<span data-ttu-id="c6c7c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6c7c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6c7c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c7c-127">Request body</span></span>
<span data-ttu-id="c6c7c-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="c6c7c-128">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="c6c7c-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="c6c7c-129">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="c6c7c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6c7c-130">Property</span></span>|<span data-ttu-id="c6c7c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6c7c-131">Type</span></span>|<span data-ttu-id="c6c7c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6c7c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6c7c-133">id</span><span class="sxs-lookup"><span data-stu-id="c6c7c-133">id</span></span>|<span data-ttu-id="c6c7c-134">String</span><span class="sxs-lookup"><span data-stu-id="c6c7c-134">String</span></span>|<span data-ttu-id="c6c7c-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c6c7c-135">Not yet documented</span></span>|
|<span data-ttu-id="c6c7c-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="c6c7c-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="c6c7c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6c7c-137">DateTimeOffset</span></span>|<span data-ttu-id="c6c7c-138">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c6c7c-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="c6c7c-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="c6c7c-139">partnerState</span></span>|[<span data-ttu-id="c6c7c-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="c6c7c-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="c6c7c-141">Estado de parceiro deste locatário.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-141">Partner state of this tenant.</span></span> <span data-ttu-id="c6c7c-142">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="c6c7c-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="c6c7c-143">partnerAppType</span></span>|[<span data-ttu-id="c6c7c-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="c6c7c-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="c6c7c-145">Tipo de aplicativo de parceiro.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-145">Partner App type.</span></span> <span data-ttu-id="c6c7c-146">Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="c6c7c-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="c6c7c-147">singleTenantAppId</span></span>|<span data-ttu-id="c6c7c-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6c7c-148">String</span></span>|<span data-ttu-id="c6c7c-149">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="c6c7c-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="c6c7c-150">displayName</span><span class="sxs-lookup"><span data-stu-id="c6c7c-150">displayName</span></span>|<span data-ttu-id="c6c7c-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6c7c-151">String</span></span>|<span data-ttu-id="c6c7c-152">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="c6c7c-152">Partner display name</span></span>|
|<span data-ttu-id="c6c7c-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="c6c7c-153">isConfigured</span></span>|<span data-ttu-id="c6c7c-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="c6c7c-154">Boolean</span></span>|<span data-ttu-id="c6c7c-155">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="c6c7c-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="c6c7c-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="c6c7c-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="c6c7c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6c7c-157">DateTimeOffset</span></span>|<span data-ttu-id="c6c7c-158">Data e hora em UTC quando PartnerDevices serão removidas.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="c6c7c-159">Isso tornará obsoleto em breve.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="c6c7c-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="c6c7c-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="c6c7c-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6c7c-161">DateTimeOffset</span></span>|<span data-ttu-id="c6c7c-162">Data e hora em UTC quando PartnerDevices será marcada como incompatível.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="c6c7c-163">Isso tornará obsoleto em breve.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="c6c7c-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6c7c-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="c6c7c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6c7c-165">DateTimeOffset</span></span>|<span data-ttu-id="c6c7c-166">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="c6c7c-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="c6c7c-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="c6c7c-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="c6c7c-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6c7c-168">DateTimeOffset</span></span>|<span data-ttu-id="c6c7c-169">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="c6c7c-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="c6c7c-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6c7c-170">Response</span></span>
<span data-ttu-id="c6c7c-171">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6c7c-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6c7c-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6c7c-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6c7c-173">Request</span></span>
<span data-ttu-id="c6c7c-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c6c7c-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6c7c-175">Response</span></span>
<span data-ttu-id="c6c7c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6c7c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





