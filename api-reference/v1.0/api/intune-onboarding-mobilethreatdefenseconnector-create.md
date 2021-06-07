---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 016900f4013a1dbdfa5eaba97ad7658fd44f4712
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752522"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="96a96-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="96a96-103">Create mobileThreatDefenseConnector</span></span>

<span data-ttu-id="96a96-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96a96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96a96-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96a96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96a96-106">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="96a96-106">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96a96-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96a96-107">Prerequisites</span></span>
<span data-ttu-id="96a96-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96a96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96a96-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96a96-110">Permission type</span></span>|<span data-ttu-id="96a96-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96a96-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96a96-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96a96-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96a96-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96a96-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="96a96-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96a96-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96a96-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96a96-115">Not supported.</span></span>|
|<span data-ttu-id="96a96-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96a96-116">Application</span></span>|<span data-ttu-id="96a96-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96a96-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96a96-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96a96-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="96a96-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96a96-119">Request headers</span></span>
|<span data-ttu-id="96a96-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96a96-120">Header</span></span>|<span data-ttu-id="96a96-121">Valor</span><span class="sxs-lookup"><span data-stu-id="96a96-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96a96-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="96a96-122">Authorization</span></span>|<span data-ttu-id="96a96-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96a96-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96a96-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96a96-124">Accept</span></span>|<span data-ttu-id="96a96-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96a96-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96a96-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96a96-126">Request body</span></span>
<span data-ttu-id="96a96-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="96a96-127">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="96a96-128">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="96a96-128">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="96a96-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96a96-129">Property</span></span>|<span data-ttu-id="96a96-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="96a96-130">Type</span></span>|<span data-ttu-id="96a96-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="96a96-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96a96-132">id</span><span class="sxs-lookup"><span data-stu-id="96a96-132">id</span></span>|<span data-ttu-id="96a96-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96a96-133">String</span></span>|<span data-ttu-id="96a96-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="96a96-134">Not yet documented</span></span>|
|<span data-ttu-id="96a96-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="96a96-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="96a96-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96a96-136">DateTimeOffset</span></span>|<span data-ttu-id="96a96-137">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="96a96-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="96a96-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="96a96-138">partnerState</span></span>|[<span data-ttu-id="96a96-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="96a96-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="96a96-140">Sincronização de Dados Estado do parceiro para essa conta.</span><span class="sxs-lookup"><span data-stu-id="96a96-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="96a96-141">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="96a96-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="96a96-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="96a96-142">androidEnabled</span></span>|<span data-ttu-id="96a96-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="96a96-143">Boolean</span></span>|<span data-ttu-id="96a96-144">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="96a96-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="96a96-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="96a96-145">iosEnabled</span></span>|<span data-ttu-id="96a96-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="96a96-146">Boolean</span></span>|<span data-ttu-id="96a96-147">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="96a96-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="96a96-148">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="96a96-148">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="96a96-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="96a96-149">Boolean</span></span>|<span data-ttu-id="96a96-150">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="96a96-150">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="96a96-151">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="96a96-151">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="96a96-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="96a96-152">Boolean</span></span>|<span data-ttu-id="96a96-153">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="96a96-153">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="96a96-154">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="96a96-154">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="96a96-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="96a96-155">Boolean</span></span>|<span data-ttu-id="96a96-156">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="96a96-156">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="96a96-157">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="96a96-157">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="96a96-158">Int32</span><span class="sxs-lookup"><span data-stu-id="96a96-158">Int32</span></span>|<span data-ttu-id="96a96-159">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="96a96-159">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="96a96-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a96-160">Response</span></span>
<span data-ttu-id="96a96-161">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96a96-161">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96a96-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96a96-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="96a96-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a96-163">Request</span></span>
<span data-ttu-id="96a96-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96a96-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96a96-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a96-165">Response</span></span>
<span data-ttu-id="96a96-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96a96-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




