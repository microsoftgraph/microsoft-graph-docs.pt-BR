---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30936d9ef9c89cc7859b5e649a7b125e40edf0b2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977671"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="c6d3e-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="c6d3e-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="c6d3e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6d3e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6d3e-106">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="c6d3e-106">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6d3e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6d3e-107">Prerequisites</span></span>
<span data-ttu-id="c6d3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6d3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6d3e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6d3e-110">Permission type</span></span>|<span data-ttu-id="c6d3e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c6d3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6d3e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6d3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6d3e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6d3e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c6d3e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6d3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6d3e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-115">Not supported.</span></span>|
|<span data-ttu-id="c6d3e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6d3e-116">Application</span></span>|<span data-ttu-id="c6d3e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6d3e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6d3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="c6d3e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6d3e-119">Request headers</span></span>
|<span data-ttu-id="c6d3e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6d3e-120">Header</span></span>|<span data-ttu-id="c6d3e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c6d3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6d3e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6d3e-122">Authorization</span></span>|<span data-ttu-id="c6d3e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6d3e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c6d3e-124">Accept</span></span>|<span data-ttu-id="c6d3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6d3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6d3e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6d3e-126">Request body</span></span>
<span data-ttu-id="c6d3e-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-127">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="c6d3e-128">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-128">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="c6d3e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6d3e-129">Property</span></span>|<span data-ttu-id="c6d3e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6d3e-130">Type</span></span>|<span data-ttu-id="c6d3e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6d3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6d3e-132">id</span><span class="sxs-lookup"><span data-stu-id="c6d3e-132">id</span></span>|<span data-ttu-id="c6d3e-133">String</span><span class="sxs-lookup"><span data-stu-id="c6d3e-133">String</span></span>|<span data-ttu-id="c6d3e-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c6d3e-134">Not yet documented</span></span>|
|<span data-ttu-id="c6d3e-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="c6d3e-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="c6d3e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6d3e-136">DateTimeOffset</span></span>|<span data-ttu-id="c6d3e-137">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="c6d3e-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="c6d3e-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="c6d3e-138">partnerState</span></span>|[<span data-ttu-id="c6d3e-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="c6d3e-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="c6d3e-140">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="c6d3e-141">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="c6d3e-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="c6d3e-142">androidEnabled</span></span>|<span data-ttu-id="c6d3e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6d3e-143">Boolean</span></span>|<span data-ttu-id="c6d3e-144">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="c6d3e-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="c6d3e-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="c6d3e-145">iosEnabled</span></span>|<span data-ttu-id="c6d3e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6d3e-146">Boolean</span></span>|<span data-ttu-id="c6d3e-147">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="c6d3e-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="c6d3e-148">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="c6d3e-148">windowsEnabled</span></span>|<span data-ttu-id="c6d3e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6d3e-149">Boolean</span></span>|<span data-ttu-id="c6d3e-150">Para o Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="c6d3e-150">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="c6d3e-151">macEnabled</span><span class="sxs-lookup"><span data-stu-id="c6d3e-151">macEnabled</span></span>|<span data-ttu-id="c6d3e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6d3e-152">Boolean</span></span>|<span data-ttu-id="c6d3e-153">Para Mac, Obtém ou define se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="c6d3e-153">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="c6d3e-154">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="c6d3e-154">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="c6d3e-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6d3e-155">Boolean</span></span>|<span data-ttu-id="c6d3e-156">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="c6d3e-156">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="c6d3e-157">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="c6d3e-157">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="c6d3e-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6d3e-158">Boolean</span></span>|<span data-ttu-id="c6d3e-159">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="c6d3e-159">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="c6d3e-160">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="c6d3e-160">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="c6d3e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6d3e-161">Boolean</span></span>|<span data-ttu-id="c6d3e-162">Para o Windows, defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="c6d3e-162">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="c6d3e-163">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="c6d3e-163">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="c6d3e-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6d3e-164">Boolean</span></span>|<span data-ttu-id="c6d3e-165">Para Mac, obtenha ou defina se o Intune deve receber dados do parceiro de sincronização de dados antes de marcar um dispositivo em conformidade</span><span class="sxs-lookup"><span data-stu-id="c6d3e-165">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="c6d3e-166">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="c6d3e-166">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="c6d3e-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6d3e-167">Boolean</span></span>|<span data-ttu-id="c6d3e-168">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="c6d3e-168">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="c6d3e-169">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="c6d3e-169">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="c6d3e-170">Int32</span><span class="sxs-lookup"><span data-stu-id="c6d3e-170">Int32</span></span>|<span data-ttu-id="c6d3e-171">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="c6d3e-171">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="c6d3e-172">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="c6d3e-172">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="c6d3e-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6d3e-173">Boolean</span></span>|<span data-ttu-id="c6d3e-174">Para dispositivos IOS, permite que o administrador configure se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados do Intune</span><span class="sxs-lookup"><span data-stu-id="c6d3e-174">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="c6d3e-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6d3e-175">Response</span></span>
<span data-ttu-id="c6d3e-176">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-176">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6d3e-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6d3e-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6d3e-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6d3e-178">Request</span></span>
<span data-ttu-id="c6d3e-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c6d3e-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6d3e-180">Response</span></span>
<span data-ttu-id="c6d3e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6d3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




