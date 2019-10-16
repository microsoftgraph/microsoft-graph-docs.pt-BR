---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc19a6b0dfa9a389c998ca443274b22ed7ebd194
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536557"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="eb16f-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="eb16f-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="eb16f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb16f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb16f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb16f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb16f-106">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="eb16f-106">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb16f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb16f-107">Prerequisites</span></span>
<span data-ttu-id="eb16f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb16f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb16f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb16f-110">Permission type</span></span>|<span data-ttu-id="eb16f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb16f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb16f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb16f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb16f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb16f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eb16f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb16f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb16f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb16f-115">Not supported.</span></span>|
|<span data-ttu-id="eb16f-116">Application</span><span class="sxs-lookup"><span data-stu-id="eb16f-116">Application</span></span>|<span data-ttu-id="eb16f-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb16f-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb16f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb16f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="eb16f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb16f-119">Request headers</span></span>
|<span data-ttu-id="eb16f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb16f-120">Header</span></span>|<span data-ttu-id="eb16f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb16f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb16f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb16f-122">Authorization</span></span>|<span data-ttu-id="eb16f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb16f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb16f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb16f-124">Accept</span></span>|<span data-ttu-id="eb16f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb16f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb16f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb16f-126">Request body</span></span>
<span data-ttu-id="eb16f-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="eb16f-127">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="eb16f-128">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="eb16f-128">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="eb16f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb16f-129">Property</span></span>|<span data-ttu-id="eb16f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb16f-130">Type</span></span>|<span data-ttu-id="eb16f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb16f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb16f-132">id</span><span class="sxs-lookup"><span data-stu-id="eb16f-132">id</span></span>|<span data-ttu-id="eb16f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb16f-133">String</span></span>|<span data-ttu-id="eb16f-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="eb16f-134">Not yet documented</span></span>|
|<span data-ttu-id="eb16f-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="eb16f-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="eb16f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb16f-136">DateTimeOffset</span></span>|<span data-ttu-id="eb16f-137">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="eb16f-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="eb16f-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="eb16f-138">partnerState</span></span>|[<span data-ttu-id="eb16f-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="eb16f-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="eb16f-140">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="eb16f-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="eb16f-141">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="eb16f-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="eb16f-142">androidMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="eb16f-142">androidMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="eb16f-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb16f-143">Boolean</span></span>|<span data-ttu-id="eb16f-144">Para Android, defina se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="eb16f-144">For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="eb16f-145">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="eb16f-145">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="eb16f-146">iosMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="eb16f-146">iosMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="eb16f-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb16f-147">Boolean</span></span>|<span data-ttu-id="eb16f-148">Para IOS, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="eb16f-148">For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="eb16f-149">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="eb16f-149">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="eb16f-150">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="eb16f-150">androidEnabled</span></span>|<span data-ttu-id="eb16f-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb16f-151">Boolean</span></span>|<span data-ttu-id="eb16f-152">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="eb16f-152">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="eb16f-153">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="eb16f-153">iosEnabled</span></span>|<span data-ttu-id="eb16f-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb16f-154">Boolean</span></span>|<span data-ttu-id="eb16f-155">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="eb16f-155">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="eb16f-156">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="eb16f-156">windowsEnabled</span></span>|<span data-ttu-id="eb16f-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb16f-157">Boolean</span></span>|<span data-ttu-id="eb16f-158">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="eb16f-158">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="eb16f-159">macEnabled</span><span class="sxs-lookup"><span data-stu-id="eb16f-159">macEnabled</span></span>|<span data-ttu-id="eb16f-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb16f-160">Boolean</span></span>|<span data-ttu-id="eb16f-161">Para Mac, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="eb16f-161">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="eb16f-162">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="eb16f-162">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="eb16f-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb16f-163">Boolean</span></span>|<span data-ttu-id="eb16f-164">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="eb16f-164">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="eb16f-165">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="eb16f-165">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="eb16f-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb16f-166">Boolean</span></span>|<span data-ttu-id="eb16f-167">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="eb16f-167">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="eb16f-168">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="eb16f-168">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="eb16f-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb16f-169">Boolean</span></span>|<span data-ttu-id="eb16f-170">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="eb16f-170">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="eb16f-171">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="eb16f-171">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="eb16f-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb16f-172">Boolean</span></span>|<span data-ttu-id="eb16f-173">Para Mac, obtenha ou defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="eb16f-173">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="eb16f-174">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="eb16f-174">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="eb16f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb16f-175">Boolean</span></span>|<span data-ttu-id="eb16f-176">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="eb16f-176">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="eb16f-177">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="eb16f-177">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="eb16f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="eb16f-178">Int32</span></span>|<span data-ttu-id="eb16f-179">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="eb16f-179">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="eb16f-180">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="eb16f-180">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="eb16f-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb16f-181">Boolean</span></span>|<span data-ttu-id="eb16f-182">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="eb16f-182">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="eb16f-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb16f-183">Response</span></span>
<span data-ttu-id="eb16f-184">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb16f-184">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb16f-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb16f-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb16f-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb16f-186">Request</span></span>
<span data-ttu-id="eb16f-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb16f-187">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb16f-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb16f-188">Response</span></span>
<span data-ttu-id="eb16f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb16f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






