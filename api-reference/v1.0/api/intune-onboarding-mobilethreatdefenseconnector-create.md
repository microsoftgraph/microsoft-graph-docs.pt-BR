---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35f9c4ed2166eb639c8af3ea198882b5ccbd1fee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512465"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="49ad4-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="49ad4-103">Create mobileThreatDefenseConnector</span></span>

<span data-ttu-id="49ad4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49ad4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49ad4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49ad4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49ad4-106">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="49ad4-106">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49ad4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49ad4-107">Prerequisites</span></span>
<span data-ttu-id="49ad4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49ad4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49ad4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49ad4-110">Permission type</span></span>|<span data-ttu-id="49ad4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49ad4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49ad4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49ad4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49ad4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ad4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="49ad4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49ad4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49ad4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49ad4-115">Not supported.</span></span>|
|<span data-ttu-id="49ad4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49ad4-116">Application</span></span>|<span data-ttu-id="49ad4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49ad4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49ad4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49ad4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="49ad4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49ad4-119">Request headers</span></span>
|<span data-ttu-id="49ad4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49ad4-120">Header</span></span>|<span data-ttu-id="49ad4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="49ad4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49ad4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="49ad4-122">Authorization</span></span>|<span data-ttu-id="49ad4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49ad4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49ad4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49ad4-124">Accept</span></span>|<span data-ttu-id="49ad4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49ad4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49ad4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49ad4-126">Request body</span></span>
<span data-ttu-id="49ad4-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="49ad4-127">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="49ad4-128">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="49ad4-128">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="49ad4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49ad4-129">Property</span></span>|<span data-ttu-id="49ad4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="49ad4-130">Type</span></span>|<span data-ttu-id="49ad4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="49ad4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49ad4-132">id</span><span class="sxs-lookup"><span data-stu-id="49ad4-132">id</span></span>|<span data-ttu-id="49ad4-133">String</span><span class="sxs-lookup"><span data-stu-id="49ad4-133">String</span></span>|<span data-ttu-id="49ad4-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="49ad4-134">Not yet documented</span></span>|
|<span data-ttu-id="49ad4-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="49ad4-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="49ad4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49ad4-136">DateTimeOffset</span></span>|<span data-ttu-id="49ad4-137">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="49ad4-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="49ad4-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="49ad4-138">partnerState</span></span>|[<span data-ttu-id="49ad4-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="49ad4-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="49ad4-140">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="49ad4-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="49ad4-141">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="49ad4-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="49ad4-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="49ad4-142">androidEnabled</span></span>|<span data-ttu-id="49ad4-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="49ad4-143">Boolean</span></span>|<span data-ttu-id="49ad4-144">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="49ad4-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="49ad4-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="49ad4-145">iosEnabled</span></span>|<span data-ttu-id="49ad4-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="49ad4-146">Boolean</span></span>|<span data-ttu-id="49ad4-147">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="49ad4-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="49ad4-148">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="49ad4-148">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="49ad4-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="49ad4-149">Boolean</span></span>|<span data-ttu-id="49ad4-150">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="49ad4-150">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="49ad4-151">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="49ad4-151">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="49ad4-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="49ad4-152">Boolean</span></span>|<span data-ttu-id="49ad4-153">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="49ad4-153">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="49ad4-154">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="49ad4-154">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="49ad4-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="49ad4-155">Boolean</span></span>|<span data-ttu-id="49ad4-156">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="49ad4-156">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="49ad4-157">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="49ad4-157">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="49ad4-158">Int32</span><span class="sxs-lookup"><span data-stu-id="49ad4-158">Int32</span></span>|<span data-ttu-id="49ad4-159">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="49ad4-159">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="49ad4-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="49ad4-160">Response</span></span>
<span data-ttu-id="49ad4-161">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49ad4-161">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49ad4-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49ad4-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="49ad4-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49ad4-163">Request</span></span>
<span data-ttu-id="49ad4-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49ad4-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="49ad4-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="49ad4-165">Response</span></span>
<span data-ttu-id="49ad4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49ad4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




