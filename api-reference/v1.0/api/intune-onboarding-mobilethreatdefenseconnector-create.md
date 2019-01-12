---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3336c03f86ac7b6d9b926780fccd5cc9e60d5db2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950673"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="4b338-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="4b338-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="4b338-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4b338-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b338-105">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="4b338-105">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b338-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b338-106">Prerequisites</span></span>
<span data-ttu-id="4b338-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b338-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b338-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b338-109">Permission type</span></span>|<span data-ttu-id="4b338-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b338-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b338-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b338-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4b338-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b338-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4b338-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b338-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b338-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b338-114">Not supported.</span></span>|
|<span data-ttu-id="4b338-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b338-115">Application</span></span>|<span data-ttu-id="4b338-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b338-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b338-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b338-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="4b338-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b338-118">Request headers</span></span>
|<span data-ttu-id="4b338-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b338-119">Header</span></span>|<span data-ttu-id="4b338-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4b338-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b338-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b338-121">Authorization</span></span>|<span data-ttu-id="4b338-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b338-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b338-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b338-123">Accept</span></span>|<span data-ttu-id="4b338-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4b338-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b338-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b338-125">Request body</span></span>
<span data-ttu-id="4b338-126">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="4b338-126">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="4b338-127">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="4b338-127">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="4b338-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b338-128">Property</span></span>|<span data-ttu-id="4b338-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b338-129">Type</span></span>|<span data-ttu-id="4b338-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b338-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b338-131">id</span><span class="sxs-lookup"><span data-stu-id="4b338-131">id</span></span>|<span data-ttu-id="4b338-132">String</span><span class="sxs-lookup"><span data-stu-id="4b338-132">String</span></span>|<span data-ttu-id="4b338-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4b338-133">Not yet documented</span></span>|
|<span data-ttu-id="4b338-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="4b338-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="4b338-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b338-135">DateTimeOffset</span></span>|<span data-ttu-id="4b338-136">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="4b338-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="4b338-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="4b338-137">partnerState</span></span>|[<span data-ttu-id="4b338-138">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="4b338-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="4b338-139">Estado de parceiro de sincronização de dados para essa conta.</span><span class="sxs-lookup"><span data-stu-id="4b338-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="4b338-140">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="4b338-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="4b338-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="4b338-141">androidEnabled</span></span>|<span data-ttu-id="4b338-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b338-142">Boolean</span></span>|<span data-ttu-id="4b338-143">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="4b338-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4b338-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="4b338-144">iosEnabled</span></span>|<span data-ttu-id="4b338-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b338-145">Boolean</span></span>|<span data-ttu-id="4b338-146">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="4b338-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4b338-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4b338-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4b338-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b338-148">Boolean</span></span>|<span data-ttu-id="4b338-149">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="4b338-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4b338-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4b338-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4b338-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b338-151">Boolean</span></span>|<span data-ttu-id="4b338-152">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="4b338-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4b338-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="4b338-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="4b338-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b338-154">Boolean</span></span>|<span data-ttu-id="4b338-155">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="4b338-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="4b338-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="4b338-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="4b338-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4b338-157">Int32</span></span>|<span data-ttu-id="4b338-158">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="4b338-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="4b338-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b338-159">Response</span></span>
<span data-ttu-id="4b338-160">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b338-160">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b338-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b338-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b338-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b338-162">Request</span></span>
<span data-ttu-id="4b338-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b338-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b338-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b338-164">Response</span></span>
<span data-ttu-id="4b338-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b338-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



