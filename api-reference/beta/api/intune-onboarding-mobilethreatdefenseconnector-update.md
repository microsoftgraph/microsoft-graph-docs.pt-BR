---
title: Atualizar mobileThreatDefenseConnector
description: Atualiza as propriedades de um objeto mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b19b61ffc8a9d66cb58ed37e0a16e93240f1ce31
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971742"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="2b54b-103">Atualizar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="2b54b-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="2b54b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b54b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b54b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b54b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b54b-106">Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="2b54b-106">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b54b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b54b-107">Prerequisites</span></span>
<span data-ttu-id="2b54b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b54b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b54b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b54b-110">Permission type</span></span>|<span data-ttu-id="2b54b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b54b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b54b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b54b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b54b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b54b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2b54b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b54b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b54b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b54b-115">Not supported.</span></span>|
|<span data-ttu-id="2b54b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b54b-116">Application</span></span>|<span data-ttu-id="2b54b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b54b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b54b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b54b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="2b54b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b54b-119">Request headers</span></span>
|<span data-ttu-id="2b54b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b54b-120">Header</span></span>|<span data-ttu-id="2b54b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2b54b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b54b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b54b-122">Authorization</span></span>|<span data-ttu-id="2b54b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b54b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b54b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b54b-124">Accept</span></span>|<span data-ttu-id="2b54b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2b54b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b54b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b54b-126">Request body</span></span>
<span data-ttu-id="2b54b-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="2b54b-127">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="2b54b-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="2b54b-128">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="2b54b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b54b-129">Property</span></span>|<span data-ttu-id="2b54b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b54b-130">Type</span></span>|<span data-ttu-id="2b54b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b54b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b54b-132">id</span><span class="sxs-lookup"><span data-stu-id="2b54b-132">id</span></span>|<span data-ttu-id="2b54b-133">String</span><span class="sxs-lookup"><span data-stu-id="2b54b-133">String</span></span>|<span data-ttu-id="2b54b-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2b54b-134">Not yet documented</span></span>|
|<span data-ttu-id="2b54b-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="2b54b-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="2b54b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b54b-136">DateTimeOffset</span></span>|<span data-ttu-id="2b54b-137">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="2b54b-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="2b54b-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="2b54b-138">partnerState</span></span>|[<span data-ttu-id="2b54b-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="2b54b-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="2b54b-140">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="2b54b-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="2b54b-141">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="2b54b-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="2b54b-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="2b54b-142">androidEnabled</span></span>|<span data-ttu-id="2b54b-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b54b-143">Boolean</span></span>|<span data-ttu-id="2b54b-144">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="2b54b-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="2b54b-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="2b54b-145">iosEnabled</span></span>|<span data-ttu-id="2b54b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b54b-146">Boolean</span></span>|<span data-ttu-id="2b54b-147">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="2b54b-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="2b54b-148">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="2b54b-148">windowsEnabled</span></span>|<span data-ttu-id="2b54b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b54b-149">Boolean</span></span>|<span data-ttu-id="2b54b-150">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="2b54b-150">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="2b54b-151">macEnabled</span><span class="sxs-lookup"><span data-stu-id="2b54b-151">macEnabled</span></span>|<span data-ttu-id="2b54b-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b54b-152">Boolean</span></span>|<span data-ttu-id="2b54b-153">Para Mac, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="2b54b-153">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="2b54b-154">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2b54b-154">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2b54b-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b54b-155">Boolean</span></span>|<span data-ttu-id="2b54b-156">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="2b54b-156">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="2b54b-157">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2b54b-157">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2b54b-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b54b-158">Boolean</span></span>|<span data-ttu-id="2b54b-159">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="2b54b-159">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="2b54b-160">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2b54b-160">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2b54b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b54b-161">Boolean</span></span>|<span data-ttu-id="2b54b-162">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="2b54b-162">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="2b54b-163">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2b54b-163">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2b54b-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b54b-164">Boolean</span></span>|<span data-ttu-id="2b54b-165">Para Mac, obtenha ou defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="2b54b-165">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="2b54b-166">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="2b54b-166">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="2b54b-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b54b-167">Boolean</span></span>|<span data-ttu-id="2b54b-168">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="2b54b-168">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="2b54b-169">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="2b54b-169">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="2b54b-170">Int32</span><span class="sxs-lookup"><span data-stu-id="2b54b-170">Int32</span></span>|<span data-ttu-id="2b54b-171">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="2b54b-171">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="2b54b-172">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="2b54b-172">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="2b54b-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b54b-173">Boolean</span></span>|<span data-ttu-id="2b54b-174">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="2b54b-174">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="2b54b-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b54b-175">Response</span></span>
<span data-ttu-id="2b54b-176">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b54b-176">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b54b-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b54b-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b54b-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b54b-178">Request</span></span>
<span data-ttu-id="2b54b-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b54b-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b54b-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b54b-180">Response</span></span>
<span data-ttu-id="2b54b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b54b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




