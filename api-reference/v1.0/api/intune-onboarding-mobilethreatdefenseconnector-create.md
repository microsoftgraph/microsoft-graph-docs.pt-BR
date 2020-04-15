---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 17717aef6ccc55b51c986f757c5112db436d1ca7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462886"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="3eb70-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="3eb70-103">Create mobileThreatDefenseConnector</span></span>

<span data-ttu-id="3eb70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eb70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3eb70-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3eb70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eb70-106">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="3eb70-106">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3eb70-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3eb70-107">Prerequisites</span></span>
<span data-ttu-id="3eb70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eb70-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3eb70-110">Permission type</span></span>|<span data-ttu-id="3eb70-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3eb70-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eb70-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3eb70-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3eb70-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb70-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3eb70-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3eb70-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eb70-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eb70-115">Not supported.</span></span>|
|<span data-ttu-id="3eb70-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3eb70-116">Application</span></span>|<span data-ttu-id="3eb70-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eb70-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eb70-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3eb70-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="3eb70-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb70-119">Request headers</span></span>
|<span data-ttu-id="3eb70-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3eb70-120">Header</span></span>|<span data-ttu-id="3eb70-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3eb70-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eb70-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3eb70-122">Authorization</span></span>|<span data-ttu-id="3eb70-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3eb70-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eb70-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3eb70-124">Accept</span></span>|<span data-ttu-id="3eb70-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3eb70-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eb70-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb70-126">Request body</span></span>
<span data-ttu-id="3eb70-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="3eb70-127">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="3eb70-128">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="3eb70-128">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="3eb70-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3eb70-129">Property</span></span>|<span data-ttu-id="3eb70-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3eb70-130">Type</span></span>|<span data-ttu-id="3eb70-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eb70-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eb70-132">id</span><span class="sxs-lookup"><span data-stu-id="3eb70-132">id</span></span>|<span data-ttu-id="3eb70-133">String</span><span class="sxs-lookup"><span data-stu-id="3eb70-133">String</span></span>|<span data-ttu-id="3eb70-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3eb70-134">Not yet documented</span></span>|
|<span data-ttu-id="3eb70-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="3eb70-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="3eb70-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eb70-136">DateTimeOffset</span></span>|<span data-ttu-id="3eb70-137">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="3eb70-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="3eb70-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="3eb70-138">partnerState</span></span>|[<span data-ttu-id="3eb70-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="3eb70-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="3eb70-140">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="3eb70-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="3eb70-141">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="3eb70-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="3eb70-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="3eb70-142">androidEnabled</span></span>|<span data-ttu-id="3eb70-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb70-143">Boolean</span></span>|<span data-ttu-id="3eb70-144">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="3eb70-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="3eb70-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="3eb70-145">iosEnabled</span></span>|<span data-ttu-id="3eb70-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb70-146">Boolean</span></span>|<span data-ttu-id="3eb70-147">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="3eb70-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="3eb70-148">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="3eb70-148">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="3eb70-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb70-149">Boolean</span></span>|<span data-ttu-id="3eb70-150">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="3eb70-150">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="3eb70-151">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="3eb70-151">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="3eb70-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb70-152">Boolean</span></span>|<span data-ttu-id="3eb70-153">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="3eb70-153">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="3eb70-154">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="3eb70-154">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="3eb70-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="3eb70-155">Boolean</span></span>|<span data-ttu-id="3eb70-156">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="3eb70-156">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="3eb70-157">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="3eb70-157">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="3eb70-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3eb70-158">Int32</span></span>|<span data-ttu-id="3eb70-159">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="3eb70-159">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="3eb70-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eb70-160">Response</span></span>
<span data-ttu-id="3eb70-161">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3eb70-161">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eb70-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3eb70-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="3eb70-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb70-163">Request</span></span>
<span data-ttu-id="3eb70-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3eb70-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
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

### <a name="response"></a><span data-ttu-id="3eb70-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eb70-165">Response</span></span>
<span data-ttu-id="3eb70-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3eb70-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






