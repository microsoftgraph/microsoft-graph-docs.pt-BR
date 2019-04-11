---
title: Atualizar mobileThreatDefenseConnector
description: Atualiza as propriedades de um objeto mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d420b41c4de711a501420ed0ec05b4f65f03a149
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776084"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="b2c14-103">Atualizar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="b2c14-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="b2c14-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2c14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2c14-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2c14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2c14-106">Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b2c14-106">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2c14-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2c14-107">Prerequisites</span></span>
<span data-ttu-id="b2c14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2c14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2c14-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2c14-110">Permission type</span></span>|<span data-ttu-id="b2c14-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2c14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2c14-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2c14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2c14-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2c14-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b2c14-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2c14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2c14-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2c14-115">Not supported.</span></span>|
|<span data-ttu-id="b2c14-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2c14-116">Application</span></span>|<span data-ttu-id="b2c14-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2c14-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2c14-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2c14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="b2c14-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c14-119">Request headers</span></span>
|<span data-ttu-id="b2c14-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2c14-120">Header</span></span>|<span data-ttu-id="b2c14-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2c14-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2c14-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2c14-122">Authorization</span></span>|<span data-ttu-id="b2c14-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2c14-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2c14-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2c14-124">Accept</span></span>|<span data-ttu-id="b2c14-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2c14-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2c14-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c14-126">Request body</span></span>
<span data-ttu-id="b2c14-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b2c14-127">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="b2c14-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b2c14-128">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="b2c14-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2c14-129">Property</span></span>|<span data-ttu-id="b2c14-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2c14-130">Type</span></span>|<span data-ttu-id="b2c14-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2c14-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2c14-132">id</span><span class="sxs-lookup"><span data-stu-id="b2c14-132">id</span></span>|<span data-ttu-id="b2c14-133">String</span><span class="sxs-lookup"><span data-stu-id="b2c14-133">String</span></span>|<span data-ttu-id="b2c14-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b2c14-134">Not yet documented</span></span>|
|<span data-ttu-id="b2c14-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="b2c14-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="b2c14-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2c14-136">DateTimeOffset</span></span>|<span data-ttu-id="b2c14-137">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="b2c14-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="b2c14-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="b2c14-138">partnerState</span></span>|[<span data-ttu-id="b2c14-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="b2c14-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="b2c14-140">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="b2c14-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="b2c14-141">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="b2c14-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="b2c14-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="b2c14-142">androidEnabled</span></span>|<span data-ttu-id="b2c14-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2c14-143">Boolean</span></span>|<span data-ttu-id="b2c14-144">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="b2c14-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b2c14-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="b2c14-145">iosEnabled</span></span>|<span data-ttu-id="b2c14-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2c14-146">Boolean</span></span>|<span data-ttu-id="b2c14-147">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="b2c14-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b2c14-148">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="b2c14-148">windowsEnabled</span></span>|<span data-ttu-id="b2c14-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2c14-149">Boolean</span></span>|<span data-ttu-id="b2c14-150">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="b2c14-150">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b2c14-151">macEnabled</span><span class="sxs-lookup"><span data-stu-id="b2c14-151">macEnabled</span></span>|<span data-ttu-id="b2c14-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2c14-152">Boolean</span></span>|<span data-ttu-id="b2c14-153">Para Mac, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="b2c14-153">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b2c14-154">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b2c14-154">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b2c14-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2c14-155">Boolean</span></span>|<span data-ttu-id="b2c14-156">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="b2c14-156">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b2c14-157">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b2c14-157">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b2c14-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2c14-158">Boolean</span></span>|<span data-ttu-id="b2c14-159">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="b2c14-159">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b2c14-160">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b2c14-160">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b2c14-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2c14-161">Boolean</span></span>|<span data-ttu-id="b2c14-162">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="b2c14-162">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b2c14-163">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b2c14-163">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b2c14-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2c14-164">Boolean</span></span>|<span data-ttu-id="b2c14-165">Para Mac, obtenha ou defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="b2c14-165">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b2c14-166">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="b2c14-166">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="b2c14-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2c14-167">Boolean</span></span>|<span data-ttu-id="b2c14-168">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="b2c14-168">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="b2c14-169">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="b2c14-169">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="b2c14-170">Int32</span><span class="sxs-lookup"><span data-stu-id="b2c14-170">Int32</span></span>|<span data-ttu-id="b2c14-171">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="b2c14-171">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="b2c14-172">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="b2c14-172">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="b2c14-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="b2c14-173">Boolean</span></span>|<span data-ttu-id="b2c14-174">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="b2c14-174">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="b2c14-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2c14-175">Response</span></span>
<span data-ttu-id="b2c14-176">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2c14-176">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2c14-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2c14-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2c14-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c14-178">Request</span></span>
<span data-ttu-id="b2c14-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2c14-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 622

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```

### <a name="response"></a><span data-ttu-id="b2c14-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2c14-180">Response</span></span>
<span data-ttu-id="b2c14-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2c14-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```





