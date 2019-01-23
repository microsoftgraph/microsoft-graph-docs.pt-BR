---
title: Criar deviceManagementPartner
description: Criar um novo objeto deviceManagementPartner.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e343b507d81d4d33ca61845e5e9810a09ca700b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412769"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="51dc8-103">Criar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="51dc8-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="51dc8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="51dc8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="51dc8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51dc8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51dc8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="51dc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51dc8-107">Criar um novo objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="51dc8-107">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51dc8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51dc8-108">Prerequisites</span></span>
<span data-ttu-id="51dc8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="51dc8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51dc8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51dc8-111">Permission type</span></span>|<span data-ttu-id="51dc8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51dc8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51dc8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51dc8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51dc8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51dc8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="51dc8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51dc8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51dc8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51dc8-116">Not supported.</span></span>|
|<span data-ttu-id="51dc8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51dc8-117">Application</span></span>|<span data-ttu-id="51dc8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51dc8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51dc8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51dc8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="51dc8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51dc8-120">Request headers</span></span>
|<span data-ttu-id="51dc8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51dc8-121">Header</span></span>|<span data-ttu-id="51dc8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="51dc8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51dc8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51dc8-123">Authorization</span></span>|<span data-ttu-id="51dc8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51dc8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51dc8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51dc8-125">Accept</span></span>|<span data-ttu-id="51dc8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51dc8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51dc8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51dc8-127">Request body</span></span>
<span data-ttu-id="51dc8-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="51dc8-128">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="51dc8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="51dc8-129">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="51dc8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51dc8-130">Property</span></span>|<span data-ttu-id="51dc8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="51dc8-131">Type</span></span>|<span data-ttu-id="51dc8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="51dc8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51dc8-133">id</span><span class="sxs-lookup"><span data-stu-id="51dc8-133">id</span></span>|<span data-ttu-id="51dc8-134">String</span><span class="sxs-lookup"><span data-stu-id="51dc8-134">String</span></span>|<span data-ttu-id="51dc8-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="51dc8-135">Not yet documented</span></span>|
|<span data-ttu-id="51dc8-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="51dc8-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="51dc8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51dc8-137">DateTimeOffset</span></span>|<span data-ttu-id="51dc8-138">Carimbo de data/hora da última pulsação após a opção de administrador habilitado conectar-se ao parceiro de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="51dc8-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="51dc8-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="51dc8-139">partnerState</span></span>|[<span data-ttu-id="51dc8-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="51dc8-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="51dc8-141">Estado de parceiro deste locatário.</span><span class="sxs-lookup"><span data-stu-id="51dc8-141">Partner state of this tenant.</span></span> <span data-ttu-id="51dc8-142">Os possíveis valores são: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="51dc8-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="51dc8-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="51dc8-143">partnerAppType</span></span>|[<span data-ttu-id="51dc8-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="51dc8-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="51dc8-145">Tipo de aplicativo de parceiro.</span><span class="sxs-lookup"><span data-stu-id="51dc8-145">Partner App type.</span></span> <span data-ttu-id="51dc8-146">Os valores possíveis são: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="51dc8-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="51dc8-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="51dc8-147">singleTenantAppId</span></span>|<span data-ttu-id="51dc8-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51dc8-148">String</span></span>|<span data-ttu-id="51dc8-149">Id do aplicativo do único locatário do parceiro</span><span class="sxs-lookup"><span data-stu-id="51dc8-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="51dc8-150">displayName</span><span class="sxs-lookup"><span data-stu-id="51dc8-150">displayName</span></span>|<span data-ttu-id="51dc8-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51dc8-151">String</span></span>|<span data-ttu-id="51dc8-152">Nome de exibição de parceiro</span><span class="sxs-lookup"><span data-stu-id="51dc8-152">Partner display name</span></span>|
|<span data-ttu-id="51dc8-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="51dc8-153">isConfigured</span></span>|<span data-ttu-id="51dc8-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="51dc8-154">Boolean</span></span>|<span data-ttu-id="51dc8-155">Se o parceiro de gerenciamento de dispositivo está configurado ou não</span><span class="sxs-lookup"><span data-stu-id="51dc8-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="51dc8-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="51dc8-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="51dc8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51dc8-157">DateTimeOffset</span></span>|<span data-ttu-id="51dc8-158">Data e hora em UTC quando PartnerDevices serão removidas.</span><span class="sxs-lookup"><span data-stu-id="51dc8-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="51dc8-159">Isso tornará obsoleto em breve.</span><span class="sxs-lookup"><span data-stu-id="51dc8-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="51dc8-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="51dc8-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="51dc8-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51dc8-161">DateTimeOffset</span></span>|<span data-ttu-id="51dc8-162">Data e hora em UTC quando PartnerDevices será marcada como incompatível.</span><span class="sxs-lookup"><span data-stu-id="51dc8-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="51dc8-163">Isso tornará obsoleto em breve.</span><span class="sxs-lookup"><span data-stu-id="51dc8-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="51dc8-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="51dc8-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="51dc8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51dc8-165">DateTimeOffset</span></span>|<span data-ttu-id="51dc8-166">DateTime no UTC quando PartnerDevices for removido</span><span class="sxs-lookup"><span data-stu-id="51dc8-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="51dc8-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="51dc8-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="51dc8-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51dc8-168">DateTimeOffset</span></span>|<span data-ttu-id="51dc8-169">DateTime no UTC quando PartnerDevices for marcado como não compatível</span><span class="sxs-lookup"><span data-stu-id="51dc8-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="51dc8-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="51dc8-170">Response</span></span>
<span data-ttu-id="51dc8-171">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51dc8-171">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51dc8-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51dc8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="51dc8-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51dc8-173">Request</span></span>
<span data-ttu-id="51dc8-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51dc8-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
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

### <a name="response"></a><span data-ttu-id="51dc8-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="51dc8-175">Response</span></span>
<span data-ttu-id="51dc8-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51dc8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




