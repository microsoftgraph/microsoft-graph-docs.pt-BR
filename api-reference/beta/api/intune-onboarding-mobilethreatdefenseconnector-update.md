---
title: Atualizar mobileThreatDefenseConnector
description: Atualiza as propriedades de um objeto mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b43e15722129099c84af1877ffa29fd070b5370c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43377699"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="81830-103">Atualizar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="81830-103">Update mobileThreatDefenseConnector</span></span>

<span data-ttu-id="81830-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81830-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81830-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81830-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81830-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81830-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81830-107">Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="81830-107">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81830-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81830-108">Prerequisites</span></span>
<span data-ttu-id="81830-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81830-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81830-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81830-111">Permission type</span></span>|<span data-ttu-id="81830-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81830-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81830-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81830-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81830-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81830-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="81830-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81830-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81830-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81830-116">Not supported.</span></span>|
|<span data-ttu-id="81830-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81830-117">Application</span></span>|<span data-ttu-id="81830-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81830-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81830-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81830-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="81830-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81830-120">Request headers</span></span>
|<span data-ttu-id="81830-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81830-121">Header</span></span>|<span data-ttu-id="81830-122">Valor</span><span class="sxs-lookup"><span data-stu-id="81830-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81830-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81830-123">Authorization</span></span>|<span data-ttu-id="81830-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81830-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81830-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81830-125">Accept</span></span>|<span data-ttu-id="81830-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81830-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81830-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81830-127">Request body</span></span>
<span data-ttu-id="81830-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="81830-128">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="81830-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="81830-129">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="81830-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81830-130">Property</span></span>|<span data-ttu-id="81830-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="81830-131">Type</span></span>|<span data-ttu-id="81830-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="81830-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81830-133">id</span><span class="sxs-lookup"><span data-stu-id="81830-133">id</span></span>|<span data-ttu-id="81830-134">String</span><span class="sxs-lookup"><span data-stu-id="81830-134">String</span></span>|<span data-ttu-id="81830-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="81830-135">Not yet documented</span></span>|
|<span data-ttu-id="81830-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="81830-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="81830-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81830-137">DateTimeOffset</span></span>|<span data-ttu-id="81830-138">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="81830-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="81830-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="81830-139">partnerState</span></span>|[<span data-ttu-id="81830-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="81830-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="81830-141">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="81830-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="81830-142">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="81830-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="81830-143">androidMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="81830-143">androidMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="81830-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-144">Boolean</span></span>|<span data-ttu-id="81830-145">Para Android, defina se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="81830-145">For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="81830-146">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="81830-146">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="81830-147">iosMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="81830-147">iosMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="81830-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-148">Boolean</span></span>|<span data-ttu-id="81830-149">Para IOS, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="81830-149">For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="81830-150">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="81830-150">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="81830-151">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="81830-151">androidEnabled</span></span>|<span data-ttu-id="81830-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-152">Boolean</span></span>|<span data-ttu-id="81830-153">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="81830-153">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="81830-154">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="81830-154">iosEnabled</span></span>|<span data-ttu-id="81830-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-155">Boolean</span></span>|<span data-ttu-id="81830-156">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="81830-156">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="81830-157">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="81830-157">windowsEnabled</span></span>|<span data-ttu-id="81830-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-158">Boolean</span></span>|<span data-ttu-id="81830-159">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="81830-159">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="81830-160">macEnabled</span><span class="sxs-lookup"><span data-stu-id="81830-160">macEnabled</span></span>|<span data-ttu-id="81830-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-161">Boolean</span></span>|<span data-ttu-id="81830-162">Para Mac, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="81830-162">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="81830-163">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="81830-163">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="81830-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-164">Boolean</span></span>|<span data-ttu-id="81830-165">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="81830-165">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="81830-166">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="81830-166">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="81830-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-167">Boolean</span></span>|<span data-ttu-id="81830-168">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="81830-168">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="81830-169">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="81830-169">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="81830-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-170">Boolean</span></span>|<span data-ttu-id="81830-171">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="81830-171">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="81830-172">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="81830-172">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="81830-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-173">Boolean</span></span>|<span data-ttu-id="81830-174">Para Mac, obtenha ou defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="81830-174">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="81830-175">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="81830-175">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="81830-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-176">Boolean</span></span>|<span data-ttu-id="81830-177">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="81830-177">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="81830-178">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="81830-178">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="81830-179">Int32</span><span class="sxs-lookup"><span data-stu-id="81830-179">Int32</span></span>|<span data-ttu-id="81830-180">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="81830-180">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="81830-181">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="81830-181">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="81830-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="81830-182">Boolean</span></span>|<span data-ttu-id="81830-183">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="81830-183">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="81830-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="81830-184">Response</span></span>
<span data-ttu-id="81830-185">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81830-185">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81830-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81830-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="81830-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81830-187">Request</span></span>
<span data-ttu-id="81830-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81830-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 726

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
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

### <a name="response"></a><span data-ttu-id="81830-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="81830-189">Response</span></span>
<span data-ttu-id="81830-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81830-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 775

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
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



