---
title: Atualizar mobileThreatDefenseConnector
description: Atualiza as propriedades de um objeto mobileThreatDefenseConnector.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 543fb2b27347a60f633eb0e731306ddd8d5c250b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362229"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="9dc7b-103">Atualizar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="9dc7b-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="9dc7b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9dc7b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dc7b-105">Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="9dc7b-105">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9dc7b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9dc7b-106">Prerequisites</span></span>
<span data-ttu-id="9dc7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dc7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dc7b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9dc7b-109">Permission type</span></span>|<span data-ttu-id="9dc7b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9dc7b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dc7b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9dc7b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9dc7b-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dc7b-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9dc7b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9dc7b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dc7b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9dc7b-114">Not supported.</span></span>|
|<span data-ttu-id="9dc7b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9dc7b-115">Application</span></span>|<span data-ttu-id="9dc7b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9dc7b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dc7b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9dc7b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="9dc7b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9dc7b-118">Request headers</span></span>
|<span data-ttu-id="9dc7b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9dc7b-119">Header</span></span>|<span data-ttu-id="9dc7b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9dc7b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dc7b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9dc7b-121">Authorization</span></span>|<span data-ttu-id="9dc7b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9dc7b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dc7b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9dc7b-123">Accept</span></span>|<span data-ttu-id="9dc7b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9dc7b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dc7b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9dc7b-125">Request body</span></span>
<span data-ttu-id="9dc7b-126">No corpo da solicitação, forneça uma representação JSON do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="9dc7b-126">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="9dc7b-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="9dc7b-127">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="9dc7b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9dc7b-128">Property</span></span>|<span data-ttu-id="9dc7b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9dc7b-129">Type</span></span>|<span data-ttu-id="9dc7b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dc7b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dc7b-131">id</span><span class="sxs-lookup"><span data-stu-id="9dc7b-131">id</span></span>|<span data-ttu-id="9dc7b-132">String</span><span class="sxs-lookup"><span data-stu-id="9dc7b-132">String</span></span>|<span data-ttu-id="9dc7b-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9dc7b-133">Not yet documented</span></span>|
|<span data-ttu-id="9dc7b-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="9dc7b-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="9dc7b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dc7b-135">DateTimeOffset</span></span>|<span data-ttu-id="9dc7b-136">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="9dc7b-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="9dc7b-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="9dc7b-137">partnerState</span></span>|[<span data-ttu-id="9dc7b-138">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="9dc7b-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="9dc7b-139">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="9dc7b-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="9dc7b-140">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="9dc7b-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="9dc7b-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="9dc7b-141">androidEnabled</span></span>|<span data-ttu-id="9dc7b-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="9dc7b-142">Boolean</span></span>|<span data-ttu-id="9dc7b-143">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="9dc7b-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="9dc7b-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="9dc7b-144">iosEnabled</span></span>|<span data-ttu-id="9dc7b-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="9dc7b-145">Boolean</span></span>|<span data-ttu-id="9dc7b-146">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="9dc7b-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="9dc7b-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="9dc7b-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="9dc7b-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="9dc7b-148">Boolean</span></span>|<span data-ttu-id="9dc7b-149">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="9dc7b-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="9dc7b-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="9dc7b-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="9dc7b-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="9dc7b-151">Boolean</span></span>|<span data-ttu-id="9dc7b-152">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="9dc7b-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="9dc7b-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="9dc7b-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="9dc7b-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dc7b-154">Boolean</span></span>|<span data-ttu-id="9dc7b-155">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="9dc7b-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="9dc7b-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="9dc7b-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="9dc7b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="9dc7b-157">Int32</span></span>|<span data-ttu-id="9dc7b-158">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="9dc7b-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="9dc7b-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dc7b-159">Response</span></span>
<span data-ttu-id="9dc7b-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9dc7b-160">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dc7b-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9dc7b-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dc7b-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9dc7b-162">Request</span></span>
<span data-ttu-id="9dc7b-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9dc7b-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="9dc7b-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dc7b-164">Response</span></span>
<span data-ttu-id="9dc7b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9dc7b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```




