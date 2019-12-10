---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 53fcd43353fcf5267a5a69499c7f07724f7ed417
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941642"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="6744d-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="6744d-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="6744d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6744d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6744d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6744d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6744d-106">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="6744d-106">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6744d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6744d-107">Prerequisites</span></span>
<span data-ttu-id="6744d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6744d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6744d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6744d-110">Permission type</span></span>|<span data-ttu-id="6744d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6744d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6744d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6744d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6744d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6744d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6744d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6744d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6744d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6744d-115">Not supported.</span></span>|
|<span data-ttu-id="6744d-116">Application</span><span class="sxs-lookup"><span data-stu-id="6744d-116">Application</span></span>|<span data-ttu-id="6744d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6744d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6744d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6744d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="6744d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6744d-119">Request headers</span></span>
|<span data-ttu-id="6744d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6744d-120">Header</span></span>|<span data-ttu-id="6744d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6744d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6744d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6744d-122">Authorization</span></span>|<span data-ttu-id="6744d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6744d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6744d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6744d-124">Accept</span></span>|<span data-ttu-id="6744d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6744d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6744d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6744d-126">Request body</span></span>
<span data-ttu-id="6744d-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="6744d-127">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="6744d-128">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="6744d-128">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="6744d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6744d-129">Property</span></span>|<span data-ttu-id="6744d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6744d-130">Type</span></span>|<span data-ttu-id="6744d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6744d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6744d-132">id</span><span class="sxs-lookup"><span data-stu-id="6744d-132">id</span></span>|<span data-ttu-id="6744d-133">String</span><span class="sxs-lookup"><span data-stu-id="6744d-133">String</span></span>|<span data-ttu-id="6744d-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6744d-134">Not yet documented</span></span>|
|<span data-ttu-id="6744d-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="6744d-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="6744d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6744d-136">DateTimeOffset</span></span>|<span data-ttu-id="6744d-137">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="6744d-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="6744d-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="6744d-138">partnerState</span></span>|[<span data-ttu-id="6744d-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="6744d-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="6744d-140">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="6744d-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="6744d-141">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="6744d-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="6744d-142">androidMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="6744d-142">androidMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="6744d-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-143">Boolean</span></span>|<span data-ttu-id="6744d-144">Para Android, defina se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="6744d-144">For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="6744d-145">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="6744d-145">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="6744d-146">iosMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="6744d-146">iosMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="6744d-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-147">Boolean</span></span>|<span data-ttu-id="6744d-148">Para IOS, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="6744d-148">For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="6744d-149">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="6744d-149">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="6744d-150">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="6744d-150">androidEnabled</span></span>|<span data-ttu-id="6744d-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-151">Boolean</span></span>|<span data-ttu-id="6744d-152">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="6744d-152">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="6744d-153">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="6744d-153">iosEnabled</span></span>|<span data-ttu-id="6744d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-154">Boolean</span></span>|<span data-ttu-id="6744d-155">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="6744d-155">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="6744d-156">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="6744d-156">windowsEnabled</span></span>|<span data-ttu-id="6744d-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-157">Boolean</span></span>|<span data-ttu-id="6744d-158">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="6744d-158">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="6744d-159">macEnabled</span><span class="sxs-lookup"><span data-stu-id="6744d-159">macEnabled</span></span>|<span data-ttu-id="6744d-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-160">Boolean</span></span>|<span data-ttu-id="6744d-161">Para Mac, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="6744d-161">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="6744d-162">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="6744d-162">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="6744d-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-163">Boolean</span></span>|<span data-ttu-id="6744d-164">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="6744d-164">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="6744d-165">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="6744d-165">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="6744d-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-166">Boolean</span></span>|<span data-ttu-id="6744d-167">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="6744d-167">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="6744d-168">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="6744d-168">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="6744d-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-169">Boolean</span></span>|<span data-ttu-id="6744d-170">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="6744d-170">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="6744d-171">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="6744d-171">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="6744d-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-172">Boolean</span></span>|<span data-ttu-id="6744d-173">Para Mac, obtenha ou defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="6744d-173">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="6744d-174">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="6744d-174">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="6744d-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-175">Boolean</span></span>|<span data-ttu-id="6744d-176">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="6744d-176">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="6744d-177">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="6744d-177">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="6744d-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6744d-178">Int32</span></span>|<span data-ttu-id="6744d-179">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="6744d-179">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="6744d-180">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="6744d-180">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="6744d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="6744d-181">Boolean</span></span>|<span data-ttu-id="6744d-182">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="6744d-182">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="6744d-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="6744d-183">Response</span></span>
<span data-ttu-id="6744d-184">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6744d-184">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6744d-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6744d-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="6744d-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6744d-186">Request</span></span>
<span data-ttu-id="6744d-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6744d-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
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

### <a name="response"></a><span data-ttu-id="6744d-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="6744d-188">Response</span></span>
<span data-ttu-id="6744d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6744d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





