---
title: Atualizar mobileThreatDefenseConnector
description: Atualiza as propriedades de um objeto mobileThreatDefenseConnector.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d652e77b62c6020dd83ba9d2088c3bdd26b09a06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512444"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="54722-103">Atualizar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="54722-103">Update mobileThreatDefenseConnector</span></span>

<span data-ttu-id="54722-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54722-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54722-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54722-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54722-106">Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="54722-106">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54722-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54722-107">Prerequisites</span></span>
<span data-ttu-id="54722-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54722-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54722-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54722-110">Permission type</span></span>|<span data-ttu-id="54722-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54722-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54722-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54722-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54722-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54722-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="54722-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54722-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54722-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54722-115">Not supported.</span></span>|
|<span data-ttu-id="54722-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54722-116">Application</span></span>|<span data-ttu-id="54722-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54722-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54722-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54722-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="54722-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54722-119">Request headers</span></span>
|<span data-ttu-id="54722-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54722-120">Header</span></span>|<span data-ttu-id="54722-121">Valor</span><span class="sxs-lookup"><span data-stu-id="54722-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54722-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="54722-122">Authorization</span></span>|<span data-ttu-id="54722-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54722-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54722-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54722-124">Accept</span></span>|<span data-ttu-id="54722-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54722-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54722-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54722-126">Request body</span></span>
<span data-ttu-id="54722-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="54722-127">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="54722-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="54722-128">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="54722-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54722-129">Property</span></span>|<span data-ttu-id="54722-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="54722-130">Type</span></span>|<span data-ttu-id="54722-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="54722-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54722-132">id</span><span class="sxs-lookup"><span data-stu-id="54722-132">id</span></span>|<span data-ttu-id="54722-133">String</span><span class="sxs-lookup"><span data-stu-id="54722-133">String</span></span>|<span data-ttu-id="54722-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="54722-134">Not yet documented</span></span>|
|<span data-ttu-id="54722-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="54722-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="54722-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54722-136">DateTimeOffset</span></span>|<span data-ttu-id="54722-137">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="54722-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="54722-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="54722-138">partnerState</span></span>|[<span data-ttu-id="54722-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="54722-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="54722-140">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="54722-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="54722-141">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="54722-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="54722-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="54722-142">androidEnabled</span></span>|<span data-ttu-id="54722-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="54722-143">Boolean</span></span>|<span data-ttu-id="54722-144">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="54722-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="54722-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="54722-145">iosEnabled</span></span>|<span data-ttu-id="54722-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="54722-146">Boolean</span></span>|<span data-ttu-id="54722-147">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="54722-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="54722-148">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="54722-148">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="54722-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="54722-149">Boolean</span></span>|<span data-ttu-id="54722-150">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="54722-150">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="54722-151">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="54722-151">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="54722-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="54722-152">Boolean</span></span>|<span data-ttu-id="54722-153">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="54722-153">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="54722-154">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="54722-154">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="54722-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="54722-155">Boolean</span></span>|<span data-ttu-id="54722-156">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="54722-156">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="54722-157">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="54722-157">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="54722-158">Int32</span><span class="sxs-lookup"><span data-stu-id="54722-158">Int32</span></span>|<span data-ttu-id="54722-159">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="54722-159">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="54722-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="54722-160">Response</span></span>
<span data-ttu-id="54722-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54722-161">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54722-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54722-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="54722-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54722-163">Request</span></span>
<span data-ttu-id="54722-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54722-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="54722-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="54722-165">Response</span></span>
<span data-ttu-id="54722-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54722-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




