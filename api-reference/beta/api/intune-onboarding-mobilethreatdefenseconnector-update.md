---
title: Atualizar mobileThreatDefenseConnector
description: Atualiza as propriedades de um objeto mobileThreatDefenseConnector.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c6e55ef5a3fa57af06b1e1cb3b14ef394c27e3d8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802780"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="10f5c-103">Atualizar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="10f5c-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="10f5c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10f5c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10f5c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10f5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10f5c-106">Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="10f5c-106">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10f5c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10f5c-107">Prerequisites</span></span>
<span data-ttu-id="10f5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10f5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10f5c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10f5c-110">Permission type</span></span>|<span data-ttu-id="10f5c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10f5c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10f5c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10f5c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10f5c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10f5c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10f5c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10f5c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10f5c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10f5c-115">Not supported.</span></span>|
|<span data-ttu-id="10f5c-116">Application</span><span class="sxs-lookup"><span data-stu-id="10f5c-116">Application</span></span>|<span data-ttu-id="10f5c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10f5c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10f5c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10f5c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="10f5c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10f5c-119">Request headers</span></span>
|<span data-ttu-id="10f5c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10f5c-120">Header</span></span>|<span data-ttu-id="10f5c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="10f5c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10f5c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="10f5c-122">Authorization</span></span>|<span data-ttu-id="10f5c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10f5c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10f5c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10f5c-124">Accept</span></span>|<span data-ttu-id="10f5c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10f5c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10f5c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10f5c-126">Request body</span></span>
<span data-ttu-id="10f5c-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="10f5c-127">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="10f5c-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="10f5c-128">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="10f5c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10f5c-129">Property</span></span>|<span data-ttu-id="10f5c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="10f5c-130">Type</span></span>|<span data-ttu-id="10f5c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="10f5c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10f5c-132">id</span><span class="sxs-lookup"><span data-stu-id="10f5c-132">id</span></span>|<span data-ttu-id="10f5c-133">String</span><span class="sxs-lookup"><span data-stu-id="10f5c-133">String</span></span>|<span data-ttu-id="10f5c-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10f5c-134">Not yet documented</span></span>|
|<span data-ttu-id="10f5c-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="10f5c-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="10f5c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10f5c-136">DateTimeOffset</span></span>|<span data-ttu-id="10f5c-137">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="10f5c-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="10f5c-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="10f5c-138">partnerState</span></span>|[<span data-ttu-id="10f5c-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="10f5c-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="10f5c-140">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="10f5c-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="10f5c-141">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="10f5c-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="10f5c-142">androidMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="10f5c-142">androidMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="10f5c-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-143">Boolean</span></span>|<span data-ttu-id="10f5c-144">Para Android, defina se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="10f5c-144">For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="10f5c-145">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="10f5c-145">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="10f5c-146">iosMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="10f5c-146">iosMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="10f5c-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-147">Boolean</span></span>|<span data-ttu-id="10f5c-148">Para IOS, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de MAM (gerenciamento de aplicativo móvel).</span><span class="sxs-lookup"><span data-stu-id="10f5c-148">For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="10f5c-149">Somente um parceiro por plataforma pode ser habilitado para a avaliação de gerenciamento de aplicativo móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="10f5c-149">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="10f5c-150">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="10f5c-150">androidEnabled</span></span>|<span data-ttu-id="10f5c-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-151">Boolean</span></span>|<span data-ttu-id="10f5c-152">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="10f5c-152">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="10f5c-153">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="10f5c-153">iosEnabled</span></span>|<span data-ttu-id="10f5c-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-154">Boolean</span></span>|<span data-ttu-id="10f5c-155">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="10f5c-155">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="10f5c-156">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="10f5c-156">windowsEnabled</span></span>|<span data-ttu-id="10f5c-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-157">Boolean</span></span>|<span data-ttu-id="10f5c-158">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="10f5c-158">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="10f5c-159">macEnabled</span><span class="sxs-lookup"><span data-stu-id="10f5c-159">macEnabled</span></span>|<span data-ttu-id="10f5c-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-160">Boolean</span></span>|<span data-ttu-id="10f5c-161">Para Mac, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="10f5c-161">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="10f5c-162">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="10f5c-162">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="10f5c-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-163">Boolean</span></span>|<span data-ttu-id="10f5c-164">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="10f5c-164">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="10f5c-165">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="10f5c-165">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="10f5c-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-166">Boolean</span></span>|<span data-ttu-id="10f5c-167">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="10f5c-167">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="10f5c-168">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="10f5c-168">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="10f5c-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-169">Boolean</span></span>|<span data-ttu-id="10f5c-170">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="10f5c-170">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="10f5c-171">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="10f5c-171">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="10f5c-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-172">Boolean</span></span>|<span data-ttu-id="10f5c-173">Para Mac, obtenha ou defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="10f5c-173">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="10f5c-174">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="10f5c-174">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="10f5c-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-175">Boolean</span></span>|<span data-ttu-id="10f5c-176">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="10f5c-176">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="10f5c-177">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="10f5c-177">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="10f5c-178">Int32</span><span class="sxs-lookup"><span data-stu-id="10f5c-178">Int32</span></span>|<span data-ttu-id="10f5c-179">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="10f5c-179">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="10f5c-180">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="10f5c-180">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="10f5c-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="10f5c-181">Boolean</span></span>|<span data-ttu-id="10f5c-182">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="10f5c-182">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="10f5c-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="10f5c-183">Response</span></span>
<span data-ttu-id="10f5c-184">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10f5c-184">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10f5c-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10f5c-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="10f5c-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10f5c-186">Request</span></span>
<span data-ttu-id="10f5c-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10f5c-187">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10f5c-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="10f5c-188">Response</span></span>
<span data-ttu-id="10f5c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10f5c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




