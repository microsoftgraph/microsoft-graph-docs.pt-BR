---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c3e5cb67f0a9df95aad53ec4c1e82669d614cec6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461967"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="8cc85-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="8cc85-103">Create mobileThreatDefenseConnector</span></span>

<span data-ttu-id="8cc85-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8cc85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cc85-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cc85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cc85-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cc85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cc85-107">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="8cc85-107">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cc85-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cc85-108">Prerequisites</span></span>
<span data-ttu-id="8cc85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc85-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc85-111">Permission type</span></span>|<span data-ttu-id="8cc85-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cc85-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cc85-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8cc85-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc85-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8cc85-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc85-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc85-116">Not supported.</span></span>|
|<span data-ttu-id="8cc85-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc85-117">Application</span></span>|<span data-ttu-id="8cc85-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc85-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc85-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="8cc85-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc85-120">Request headers</span></span>
|<span data-ttu-id="8cc85-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cc85-121">Header</span></span>|<span data-ttu-id="8cc85-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8cc85-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cc85-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc85-123">Authorization</span></span>|<span data-ttu-id="8cc85-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc85-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cc85-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8cc85-125">Accept</span></span>|<span data-ttu-id="8cc85-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cc85-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc85-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc85-127">Request body</span></span>
<span data-ttu-id="8cc85-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="8cc85-128">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="8cc85-129">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="8cc85-129">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="8cc85-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cc85-130">Property</span></span>|<span data-ttu-id="8cc85-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc85-131">Type</span></span>|<span data-ttu-id="8cc85-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc85-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc85-133">id</span><span class="sxs-lookup"><span data-stu-id="8cc85-133">id</span></span>|<span data-ttu-id="8cc85-134">String</span><span class="sxs-lookup"><span data-stu-id="8cc85-134">String</span></span>|<span data-ttu-id="8cc85-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8cc85-135">Not yet documented</span></span>|
|<span data-ttu-id="8cc85-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc85-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="8cc85-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc85-137">DateTimeOffset</span></span>|<span data-ttu-id="8cc85-138">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="8cc85-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="8cc85-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="8cc85-139">partnerState</span></span>|[<span data-ttu-id="8cc85-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="8cc85-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="8cc85-141">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="8cc85-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="8cc85-142">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="8cc85-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="8cc85-143">androidMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="8cc85-143">androidMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="8cc85-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-144">Boolean</span></span>|<span data-ttu-id="8cc85-145">Para Android, defina se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="8cc85-145">For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="8cc85-146">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="8cc85-146">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="8cc85-147">iosMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="8cc85-147">iosMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="8cc85-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-148">Boolean</span></span>|<span data-ttu-id="8cc85-149">Para IOS, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="8cc85-149">For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="8cc85-150">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="8cc85-150">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="8cc85-151">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="8cc85-151">androidEnabled</span></span>|<span data-ttu-id="8cc85-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-152">Boolean</span></span>|<span data-ttu-id="8cc85-153">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="8cc85-153">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="8cc85-154">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="8cc85-154">iosEnabled</span></span>|<span data-ttu-id="8cc85-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-155">Boolean</span></span>|<span data-ttu-id="8cc85-156">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="8cc85-156">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="8cc85-157">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="8cc85-157">windowsEnabled</span></span>|<span data-ttu-id="8cc85-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-158">Boolean</span></span>|<span data-ttu-id="8cc85-159">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="8cc85-159">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="8cc85-160">macEnabled</span><span class="sxs-lookup"><span data-stu-id="8cc85-160">macEnabled</span></span>|<span data-ttu-id="8cc85-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-161">Boolean</span></span>|<span data-ttu-id="8cc85-162">Para Mac, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="8cc85-162">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="8cc85-163">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="8cc85-163">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="8cc85-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-164">Boolean</span></span>|<span data-ttu-id="8cc85-165">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="8cc85-165">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="8cc85-166">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="8cc85-166">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="8cc85-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-167">Boolean</span></span>|<span data-ttu-id="8cc85-168">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="8cc85-168">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="8cc85-169">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="8cc85-169">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="8cc85-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-170">Boolean</span></span>|<span data-ttu-id="8cc85-171">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="8cc85-171">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="8cc85-172">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="8cc85-172">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="8cc85-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-173">Boolean</span></span>|<span data-ttu-id="8cc85-174">Para Mac, obtenha ou defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="8cc85-174">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="8cc85-175">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="8cc85-175">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="8cc85-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-176">Boolean</span></span>|<span data-ttu-id="8cc85-177">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="8cc85-177">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="8cc85-178">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="8cc85-178">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="8cc85-179">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc85-179">Int32</span></span>|<span data-ttu-id="8cc85-180">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="8cc85-180">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="8cc85-181">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="8cc85-181">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="8cc85-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc85-182">Boolean</span></span>|<span data-ttu-id="8cc85-183">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="8cc85-183">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="8cc85-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc85-184">Response</span></span>
<span data-ttu-id="8cc85-185">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc85-185">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc85-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc85-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cc85-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc85-187">Request</span></span>
<span data-ttu-id="8cc85-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc85-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8cc85-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc85-189">Response</span></span>
<span data-ttu-id="8cc85-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cc85-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





