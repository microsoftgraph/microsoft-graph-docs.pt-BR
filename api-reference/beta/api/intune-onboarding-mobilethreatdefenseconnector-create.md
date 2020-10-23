---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c20146a7c6a84526382aa610d7cb632ba9eb5aef
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731187"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="989ef-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="989ef-103">Create mobileThreatDefenseConnector</span></span>

<span data-ttu-id="989ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="989ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="989ef-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="989ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="989ef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="989ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="989ef-107">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="989ef-107">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="989ef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="989ef-108">Prerequisites</span></span>
<span data-ttu-id="989ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="989ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="989ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="989ef-111">Permission type</span></span>|<span data-ttu-id="989ef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="989ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="989ef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="989ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="989ef-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="989ef-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="989ef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="989ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="989ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="989ef-116">Not supported.</span></span>|
|<span data-ttu-id="989ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="989ef-117">Application</span></span>|<span data-ttu-id="989ef-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="989ef-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="989ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="989ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="989ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="989ef-120">Request headers</span></span>
|<span data-ttu-id="989ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="989ef-121">Header</span></span>|<span data-ttu-id="989ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="989ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="989ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="989ef-123">Authorization</span></span>|<span data-ttu-id="989ef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="989ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="989ef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="989ef-125">Accept</span></span>|<span data-ttu-id="989ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="989ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="989ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="989ef-127">Request body</span></span>
<span data-ttu-id="989ef-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="989ef-128">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="989ef-129">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="989ef-129">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="989ef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="989ef-130">Property</span></span>|<span data-ttu-id="989ef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="989ef-131">Type</span></span>|<span data-ttu-id="989ef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="989ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="989ef-133">id</span><span class="sxs-lookup"><span data-stu-id="989ef-133">id</span></span>|<span data-ttu-id="989ef-134">String</span><span class="sxs-lookup"><span data-stu-id="989ef-134">String</span></span>|<span data-ttu-id="989ef-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="989ef-135">Not yet documented</span></span>|
|<span data-ttu-id="989ef-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="989ef-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="989ef-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="989ef-137">DateTimeOffset</span></span>|<span data-ttu-id="989ef-138">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="989ef-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="989ef-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="989ef-139">partnerState</span></span>|[<span data-ttu-id="989ef-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="989ef-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="989ef-141">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="989ef-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="989ef-142">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="989ef-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="989ef-143">androidMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="989ef-143">androidMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="989ef-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="989ef-144">Boolean</span></span>|<span data-ttu-id="989ef-145">Para Android, defina se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="989ef-145">For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="989ef-146">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="989ef-146">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="989ef-147">iosMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="989ef-147">iosMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="989ef-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="989ef-148">Boolean</span></span>|<span data-ttu-id="989ef-149">Para IOS, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="989ef-149">For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="989ef-150">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="989ef-150">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="989ef-151">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="989ef-151">androidEnabled</span></span>|<span data-ttu-id="989ef-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="989ef-152">Boolean</span></span>|<span data-ttu-id="989ef-153">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="989ef-153">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="989ef-154">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="989ef-154">iosEnabled</span></span>|<span data-ttu-id="989ef-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="989ef-155">Boolean</span></span>|<span data-ttu-id="989ef-156">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="989ef-156">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="989ef-157">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="989ef-157">windowsEnabled</span></span>|<span data-ttu-id="989ef-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="989ef-158">Boolean</span></span>|<span data-ttu-id="989ef-159">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="989ef-159">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="989ef-160">macEnabled</span><span class="sxs-lookup"><span data-stu-id="989ef-160">macEnabled</span></span>|<span data-ttu-id="989ef-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="989ef-161">Boolean</span></span>|<span data-ttu-id="989ef-162">Para Mac, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="989ef-162">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="989ef-163">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="989ef-163">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="989ef-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="989ef-164">Boolean</span></span>|<span data-ttu-id="989ef-165">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="989ef-165">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="989ef-166">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="989ef-166">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="989ef-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="989ef-167">Boolean</span></span>|<span data-ttu-id="989ef-168">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="989ef-168">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="989ef-169">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="989ef-169">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="989ef-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="989ef-170">Boolean</span></span>|<span data-ttu-id="989ef-171">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="989ef-171">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="989ef-172">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="989ef-172">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="989ef-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="989ef-173">Boolean</span></span>|<span data-ttu-id="989ef-174">Para Mac, obtenha ou defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="989ef-174">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="989ef-175">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="989ef-175">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="989ef-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="989ef-176">Boolean</span></span>|<span data-ttu-id="989ef-177">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="989ef-177">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="989ef-178">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="989ef-178">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="989ef-179">Int32</span><span class="sxs-lookup"><span data-stu-id="989ef-179">Int32</span></span>|<span data-ttu-id="989ef-180">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="989ef-180">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="989ef-181">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="989ef-181">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="989ef-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="989ef-182">Boolean</span></span>|<span data-ttu-id="989ef-183">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="989ef-183">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="989ef-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="989ef-184">Response</span></span>
<span data-ttu-id="989ef-185">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="989ef-185">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="989ef-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="989ef-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="989ef-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="989ef-187">Request</span></span>
<span data-ttu-id="989ef-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="989ef-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="989ef-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="989ef-189">Response</span></span>
<span data-ttu-id="989ef-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="989ef-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





