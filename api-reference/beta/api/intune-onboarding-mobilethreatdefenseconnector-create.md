---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: caed5284908a614efc9eb84ea546b42762e84028
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969820"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="5df70-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="5df70-103">Create mobileThreatDefenseConnector</span></span>

<span data-ttu-id="5df70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5df70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5df70-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5df70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5df70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5df70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5df70-107">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="5df70-107">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5df70-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5df70-108">Prerequisites</span></span>
<span data-ttu-id="5df70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5df70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5df70-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5df70-111">Permission type</span></span>|<span data-ttu-id="5df70-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5df70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5df70-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5df70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5df70-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5df70-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5df70-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5df70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5df70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5df70-116">Not supported.</span></span>|
|<span data-ttu-id="5df70-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5df70-117">Application</span></span>|<span data-ttu-id="5df70-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5df70-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5df70-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5df70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="5df70-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5df70-120">Request headers</span></span>
|<span data-ttu-id="5df70-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5df70-121">Header</span></span>|<span data-ttu-id="5df70-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5df70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5df70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5df70-123">Authorization</span></span>|<span data-ttu-id="5df70-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5df70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5df70-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5df70-125">Accept</span></span>|<span data-ttu-id="5df70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5df70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5df70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5df70-127">Request body</span></span>
<span data-ttu-id="5df70-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="5df70-128">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="5df70-129">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="5df70-129">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="5df70-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5df70-130">Property</span></span>|<span data-ttu-id="5df70-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5df70-131">Type</span></span>|<span data-ttu-id="5df70-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5df70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5df70-133">id</span><span class="sxs-lookup"><span data-stu-id="5df70-133">id</span></span>|<span data-ttu-id="5df70-134">String</span><span class="sxs-lookup"><span data-stu-id="5df70-134">String</span></span>|<span data-ttu-id="5df70-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5df70-135">Not yet documented</span></span>|
|<span data-ttu-id="5df70-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="5df70-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="5df70-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5df70-137">DateTimeOffset</span></span>|<span data-ttu-id="5df70-138">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="5df70-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="5df70-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="5df70-139">partnerState</span></span>|[<span data-ttu-id="5df70-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="5df70-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="5df70-141">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="5df70-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="5df70-142">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="5df70-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="5df70-143">androidMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="5df70-143">androidMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="5df70-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-144">Boolean</span></span>|<span data-ttu-id="5df70-145">Para Android, defina se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="5df70-145">For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="5df70-146">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="5df70-146">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="5df70-147">iosMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="5df70-147">iosMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="5df70-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-148">Boolean</span></span>|<span data-ttu-id="5df70-149">Para IOS, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="5df70-149">For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="5df70-150">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="5df70-150">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="5df70-151">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="5df70-151">androidEnabled</span></span>|<span data-ttu-id="5df70-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-152">Boolean</span></span>|<span data-ttu-id="5df70-153">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="5df70-153">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="5df70-154">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="5df70-154">iosEnabled</span></span>|<span data-ttu-id="5df70-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-155">Boolean</span></span>|<span data-ttu-id="5df70-156">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="5df70-156">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="5df70-157">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="5df70-157">windowsEnabled</span></span>|<span data-ttu-id="5df70-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-158">Boolean</span></span>|<span data-ttu-id="5df70-159">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="5df70-159">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="5df70-160">macEnabled</span><span class="sxs-lookup"><span data-stu-id="5df70-160">macEnabled</span></span>|<span data-ttu-id="5df70-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-161">Boolean</span></span>|<span data-ttu-id="5df70-162">Para Mac, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="5df70-162">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="5df70-163">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="5df70-163">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="5df70-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-164">Boolean</span></span>|<span data-ttu-id="5df70-165">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="5df70-165">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="5df70-166">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="5df70-166">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="5df70-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-167">Boolean</span></span>|<span data-ttu-id="5df70-168">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="5df70-168">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="5df70-169">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="5df70-169">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="5df70-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-170">Boolean</span></span>|<span data-ttu-id="5df70-171">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="5df70-171">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="5df70-172">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="5df70-172">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="5df70-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-173">Boolean</span></span>|<span data-ttu-id="5df70-174">Para Mac, obtenha ou defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="5df70-174">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="5df70-175">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="5df70-175">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="5df70-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-176">Boolean</span></span>|<span data-ttu-id="5df70-177">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="5df70-177">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="5df70-178">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="5df70-178">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="5df70-179">Int32</span><span class="sxs-lookup"><span data-stu-id="5df70-179">Int32</span></span>|<span data-ttu-id="5df70-180">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="5df70-180">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="5df70-181">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="5df70-181">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="5df70-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df70-182">Boolean</span></span>|<span data-ttu-id="5df70-183">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="5df70-183">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="5df70-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="5df70-184">Response</span></span>
<span data-ttu-id="5df70-185">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5df70-185">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5df70-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5df70-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="5df70-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5df70-187">Request</span></span>
<span data-ttu-id="5df70-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5df70-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5df70-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="5df70-189">Response</span></span>
<span data-ttu-id="5df70-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5df70-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






