---
title: Atualizar mobileThreatDefenseConnector
description: Atualiza as propriedades de um objeto mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8de03a90555c5d80e10bf0c64bb408c12130cba8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156874"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="980fe-103">Atualizar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="980fe-103">Update mobileThreatDefenseConnector</span></span>

<span data-ttu-id="980fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="980fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="980fe-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="980fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="980fe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="980fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="980fe-107">Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="980fe-107">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="980fe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="980fe-108">Prerequisites</span></span>
<span data-ttu-id="980fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="980fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="980fe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="980fe-111">Permission type</span></span>|<span data-ttu-id="980fe-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="980fe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="980fe-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="980fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="980fe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="980fe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="980fe-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="980fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="980fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="980fe-116">Not supported.</span></span>|
|<span data-ttu-id="980fe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="980fe-117">Application</span></span>|<span data-ttu-id="980fe-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="980fe-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="980fe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="980fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="980fe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="980fe-120">Request headers</span></span>
|<span data-ttu-id="980fe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="980fe-121">Header</span></span>|<span data-ttu-id="980fe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="980fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="980fe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="980fe-123">Authorization</span></span>|<span data-ttu-id="980fe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="980fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="980fe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="980fe-125">Accept</span></span>|<span data-ttu-id="980fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="980fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="980fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="980fe-127">Request body</span></span>
<span data-ttu-id="980fe-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="980fe-128">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="980fe-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="980fe-129">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="980fe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="980fe-130">Property</span></span>|<span data-ttu-id="980fe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="980fe-131">Type</span></span>|<span data-ttu-id="980fe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="980fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="980fe-133">id</span><span class="sxs-lookup"><span data-stu-id="980fe-133">id</span></span>|<span data-ttu-id="980fe-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="980fe-134">String</span></span>|<span data-ttu-id="980fe-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="980fe-135">Not yet documented</span></span>|
|<span data-ttu-id="980fe-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="980fe-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="980fe-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="980fe-137">DateTimeOffset</span></span>|<span data-ttu-id="980fe-138">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="980fe-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="980fe-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="980fe-139">partnerState</span></span>|[<span data-ttu-id="980fe-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="980fe-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="980fe-141">Estado do Parceiro de Sincronização de Dados para essa conta.</span><span class="sxs-lookup"><span data-stu-id="980fe-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="980fe-142">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="980fe-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="980fe-143">androidMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="980fe-143">androidMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="980fe-144">Booleano</span><span class="sxs-lookup"><span data-stu-id="980fe-144">Boolean</span></span>|<span data-ttu-id="980fe-145">Para Android, de definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações do Gerenciamento de Aplicativo Móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="980fe-145">For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="980fe-146">Somente um parceiro por plataforma pode estar habilitado para avaliação do Gerenciamento de Aplicativo Móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="980fe-146">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="980fe-147">iosMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="980fe-147">iosMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="980fe-148">Booleano</span><span class="sxs-lookup"><span data-stu-id="980fe-148">Boolean</span></span>|<span data-ttu-id="980fe-149">Para IOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações do MAM (Gerenciamento de Aplicativo Móvel).</span><span class="sxs-lookup"><span data-stu-id="980fe-149">For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="980fe-150">Somente um parceiro por plataforma pode estar habilitado para avaliação do Gerenciamento de Aplicativo Móvel (MAM).</span><span class="sxs-lookup"><span data-stu-id="980fe-150">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="980fe-151">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="980fe-151">androidEnabled</span></span>|<span data-ttu-id="980fe-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="980fe-152">Boolean</span></span>|<span data-ttu-id="980fe-153">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="980fe-153">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="980fe-154">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="980fe-154">iosEnabled</span></span>|<span data-ttu-id="980fe-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="980fe-155">Boolean</span></span>|<span data-ttu-id="980fe-156">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="980fe-156">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="980fe-157">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="980fe-157">windowsEnabled</span></span>|<span data-ttu-id="980fe-158">Booleano</span><span class="sxs-lookup"><span data-stu-id="980fe-158">Boolean</span></span>|<span data-ttu-id="980fe-159">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="980fe-159">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="980fe-160">macEnabled</span><span class="sxs-lookup"><span data-stu-id="980fe-160">macEnabled</span></span>|<span data-ttu-id="980fe-161">Booleano</span><span class="sxs-lookup"><span data-stu-id="980fe-161">Boolean</span></span>|<span data-ttu-id="980fe-162">Para Mac, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="980fe-162">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="980fe-163">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="980fe-163">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="980fe-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="980fe-164">Boolean</span></span>|<span data-ttu-id="980fe-165">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="980fe-165">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="980fe-166">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="980fe-166">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="980fe-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="980fe-167">Boolean</span></span>|<span data-ttu-id="980fe-168">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="980fe-168">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="980fe-169">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="980fe-169">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="980fe-170">Booleano</span><span class="sxs-lookup"><span data-stu-id="980fe-170">Boolean</span></span>|<span data-ttu-id="980fe-171">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo compatível</span><span class="sxs-lookup"><span data-stu-id="980fe-171">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="980fe-172">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="980fe-172">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="980fe-173">Booleano</span><span class="sxs-lookup"><span data-stu-id="980fe-173">Boolean</span></span>|<span data-ttu-id="980fe-174">Para Mac, obter ou definir se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo compatível</span><span class="sxs-lookup"><span data-stu-id="980fe-174">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="980fe-175">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="980fe-175">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="980fe-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="980fe-176">Boolean</span></span>|<span data-ttu-id="980fe-177">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="980fe-177">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="980fe-178">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="980fe-178">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="980fe-179">Int32</span><span class="sxs-lookup"><span data-stu-id="980fe-179">Int32</span></span>|<span data-ttu-id="980fe-180">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="980fe-180">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="980fe-181">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="980fe-181">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="980fe-182">Booleano</span><span class="sxs-lookup"><span data-stu-id="980fe-182">Boolean</span></span>|<span data-ttu-id="980fe-183">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="980fe-183">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="980fe-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="980fe-184">Response</span></span>
<span data-ttu-id="980fe-185">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="980fe-185">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="980fe-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="980fe-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="980fe-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="980fe-187">Request</span></span>
<span data-ttu-id="980fe-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="980fe-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="980fe-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="980fe-189">Response</span></span>
<span data-ttu-id="980fe-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="980fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




