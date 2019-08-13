---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6653d9eb4abc5705eaa8a2dff61c0a758e9a05cf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352578"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="4fbf9-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="4fbf9-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="4fbf9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4fbf9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fbf9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4fbf9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fbf9-106">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="4fbf9-106">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fbf9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4fbf9-107">Prerequisites</span></span>
<span data-ttu-id="4fbf9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fbf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fbf9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fbf9-110">Permission type</span></span>|<span data-ttu-id="4fbf9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4fbf9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fbf9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fbf9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fbf9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fbf9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4fbf9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fbf9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fbf9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fbf9-115">Not supported.</span></span>|
|<span data-ttu-id="4fbf9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4fbf9-116">Application</span></span>|<span data-ttu-id="4fbf9-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fbf9-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fbf9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fbf9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="4fbf9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fbf9-119">Request headers</span></span>
|<span data-ttu-id="4fbf9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4fbf9-120">Header</span></span>|<span data-ttu-id="4fbf9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4fbf9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fbf9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fbf9-122">Authorization</span></span>|<span data-ttu-id="4fbf9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fbf9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fbf9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4fbf9-124">Accept</span></span>|<span data-ttu-id="4fbf9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4fbf9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fbf9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4fbf9-126">Request body</span></span>
<span data-ttu-id="4fbf9-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="4fbf9-127">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="4fbf9-128">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="4fbf9-128">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="4fbf9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fbf9-129">Property</span></span>|<span data-ttu-id="4fbf9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fbf9-130">Type</span></span>|<span data-ttu-id="4fbf9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fbf9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fbf9-132">id</span><span class="sxs-lookup"><span data-stu-id="4fbf9-132">id</span></span>|<span data-ttu-id="4fbf9-133">String</span><span class="sxs-lookup"><span data-stu-id="4fbf9-133">String</span></span>|<span data-ttu-id="4fbf9-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4fbf9-134">Not yet documented</span></span>|
|<span data-ttu-id="4fbf9-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="4fbf9-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="4fbf9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fbf9-136">DateTimeOffset</span></span>|<span data-ttu-id="4fbf9-137">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="4fbf9-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="4fbf9-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="4fbf9-138">partnerState</span></span>|[<span data-ttu-id="4fbf9-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="4fbf9-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="4fbf9-140">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="4fbf9-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="4fbf9-141">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="4fbf9-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="4fbf9-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="4fbf9-142">androidEnabled</span></span>|<span data-ttu-id="4fbf9-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fbf9-143">Boolean</span></span>|<span data-ttu-id="4fbf9-144">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="4fbf9-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4fbf9-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="4fbf9-145">iosEnabled</span></span>|<span data-ttu-id="4fbf9-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fbf9-146">Boolean</span></span>|<span data-ttu-id="4fbf9-147">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="4fbf9-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4fbf9-148">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="4fbf9-148">windowsEnabled</span></span>|<span data-ttu-id="4fbf9-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fbf9-149">Boolean</span></span>|<span data-ttu-id="4fbf9-150">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="4fbf9-150">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4fbf9-151">macEnabled</span><span class="sxs-lookup"><span data-stu-id="4fbf9-151">macEnabled</span></span>|<span data-ttu-id="4fbf9-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fbf9-152">Boolean</span></span>|<span data-ttu-id="4fbf9-153">Para Mac, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="4fbf9-153">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4fbf9-154">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4fbf9-154">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4fbf9-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fbf9-155">Boolean</span></span>|<span data-ttu-id="4fbf9-156">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="4fbf9-156">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4fbf9-157">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4fbf9-157">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4fbf9-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fbf9-158">Boolean</span></span>|<span data-ttu-id="4fbf9-159">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="4fbf9-159">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4fbf9-160">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4fbf9-160">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4fbf9-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fbf9-161">Boolean</span></span>|<span data-ttu-id="4fbf9-162">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="4fbf9-162">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4fbf9-163">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4fbf9-163">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4fbf9-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fbf9-164">Boolean</span></span>|<span data-ttu-id="4fbf9-165">Para Mac, obtenha ou defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="4fbf9-165">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4fbf9-166">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="4fbf9-166">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="4fbf9-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fbf9-167">Boolean</span></span>|<span data-ttu-id="4fbf9-168">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="4fbf9-168">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="4fbf9-169">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="4fbf9-169">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="4fbf9-170">Int32</span><span class="sxs-lookup"><span data-stu-id="4fbf9-170">Int32</span></span>|<span data-ttu-id="4fbf9-171">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="4fbf9-171">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="4fbf9-172">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="4fbf9-172">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="4fbf9-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="4fbf9-173">Boolean</span></span>|<span data-ttu-id="4fbf9-174">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="4fbf9-174">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="4fbf9-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fbf9-175">Response</span></span>
<span data-ttu-id="4fbf9-176">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fbf9-176">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fbf9-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fbf9-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fbf9-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fbf9-178">Request</span></span>
<span data-ttu-id="4fbf9-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fbf9-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
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

### <a name="response"></a><span data-ttu-id="4fbf9-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fbf9-180">Response</span></span>
<span data-ttu-id="4fbf9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4fbf9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






