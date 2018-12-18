---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: tfitzmac
ms.openlocfilehash: 8bd4551c2290e5406db1e66cf3c9396a611e5b42
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358965"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="4990f-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="4990f-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="4990f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4990f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4990f-105">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="4990f-105">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4990f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4990f-106">Prerequisites</span></span>
<span data-ttu-id="4990f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4990f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4990f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4990f-109">Permission type</span></span>|<span data-ttu-id="4990f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4990f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4990f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4990f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4990f-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4990f-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4990f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4990f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4990f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4990f-114">Not supported.</span></span>|
|<span data-ttu-id="4990f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4990f-115">Application</span></span>|<span data-ttu-id="4990f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4990f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4990f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4990f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="4990f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4990f-118">Request headers</span></span>
|<span data-ttu-id="4990f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4990f-119">Header</span></span>|<span data-ttu-id="4990f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4990f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4990f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4990f-121">Authorization</span></span>|<span data-ttu-id="4990f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4990f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4990f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4990f-123">Accept</span></span>|<span data-ttu-id="4990f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4990f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4990f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4990f-125">Request body</span></span>
<span data-ttu-id="4990f-126">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="4990f-126">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="4990f-127">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="4990f-127">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="4990f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4990f-128">Property</span></span>|<span data-ttu-id="4990f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4990f-129">Type</span></span>|<span data-ttu-id="4990f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4990f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4990f-131">id</span><span class="sxs-lookup"><span data-stu-id="4990f-131">id</span></span>|<span data-ttu-id="4990f-132">String</span><span class="sxs-lookup"><span data-stu-id="4990f-132">String</span></span>|<span data-ttu-id="4990f-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4990f-133">Not yet documented</span></span>|
|<span data-ttu-id="4990f-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="4990f-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="4990f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4990f-135">DateTimeOffset</span></span>|<span data-ttu-id="4990f-136">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="4990f-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="4990f-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="4990f-137">partnerState</span></span>|[<span data-ttu-id="4990f-138">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="4990f-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="4990f-139">Estado de parceiro de sincronização de dados para essa conta.</span><span class="sxs-lookup"><span data-stu-id="4990f-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="4990f-140">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="4990f-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="4990f-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="4990f-141">androidEnabled</span></span>|<span data-ttu-id="4990f-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="4990f-142">Boolean</span></span>|<span data-ttu-id="4990f-143">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="4990f-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4990f-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="4990f-144">iosEnabled</span></span>|<span data-ttu-id="4990f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4990f-145">Boolean</span></span>|<span data-ttu-id="4990f-146">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="4990f-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4990f-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4990f-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4990f-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="4990f-148">Boolean</span></span>|<span data-ttu-id="4990f-149">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="4990f-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4990f-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4990f-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4990f-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="4990f-151">Boolean</span></span>|<span data-ttu-id="4990f-152">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="4990f-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4990f-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="4990f-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="4990f-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="4990f-154">Boolean</span></span>|<span data-ttu-id="4990f-155">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="4990f-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="4990f-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="4990f-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="4990f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4990f-157">Int32</span></span>|<span data-ttu-id="4990f-158">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="4990f-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="4990f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="4990f-159">Response</span></span>
<span data-ttu-id="4990f-160">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4990f-160">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4990f-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4990f-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="4990f-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4990f-162">Request</span></span>
<span data-ttu-id="4990f-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4990f-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4990f-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="4990f-164">Response</span></span>
<span data-ttu-id="4990f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4990f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



