---
title: Atualizar mobileThreatDefenseConnector
description: Atualiza as propriedades de um objeto mobileThreatDefenseConnector.
author: tfitzmac
ms.openlocfilehash: bd53fb377adb160db1700b088e293217bdee5292
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313941"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="d349a-103">Atualizar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="d349a-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="d349a-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d349a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d349a-105">Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="d349a-105">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d349a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d349a-106">Prerequisites</span></span>
<span data-ttu-id="d349a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d349a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d349a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d349a-109">Permission type</span></span>|<span data-ttu-id="d349a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d349a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d349a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d349a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d349a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d349a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d349a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d349a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d349a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d349a-114">Not supported.</span></span>|
|<span data-ttu-id="d349a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d349a-115">Application</span></span>|<span data-ttu-id="d349a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d349a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d349a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d349a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="d349a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d349a-118">Request headers</span></span>
|<span data-ttu-id="d349a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d349a-119">Header</span></span>|<span data-ttu-id="d349a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d349a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d349a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d349a-121">Authorization</span></span>|<span data-ttu-id="d349a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d349a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d349a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d349a-123">Accept</span></span>|<span data-ttu-id="d349a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d349a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d349a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d349a-125">Request body</span></span>
<span data-ttu-id="d349a-126">No corpo da solicitação, forneça uma representação JSON do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="d349a-126">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="d349a-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="d349a-127">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="d349a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d349a-128">Property</span></span>|<span data-ttu-id="d349a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d349a-129">Type</span></span>|<span data-ttu-id="d349a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d349a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d349a-131">id</span><span class="sxs-lookup"><span data-stu-id="d349a-131">id</span></span>|<span data-ttu-id="d349a-132">String</span><span class="sxs-lookup"><span data-stu-id="d349a-132">String</span></span>|<span data-ttu-id="d349a-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d349a-133">Not yet documented</span></span>|
|<span data-ttu-id="d349a-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="d349a-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="d349a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d349a-135">DateTimeOffset</span></span>|<span data-ttu-id="d349a-136">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="d349a-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="d349a-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="d349a-137">partnerState</span></span>|[<span data-ttu-id="d349a-138">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="d349a-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="d349a-139">Estado de parceiro de sincronização de dados para essa conta.</span><span class="sxs-lookup"><span data-stu-id="d349a-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="d349a-140">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="d349a-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="d349a-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="d349a-141">androidEnabled</span></span>|<span data-ttu-id="d349a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="d349a-142">Boolean</span></span>|<span data-ttu-id="d349a-143">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="d349a-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="d349a-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="d349a-144">iosEnabled</span></span>|<span data-ttu-id="d349a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d349a-145">Boolean</span></span>|<span data-ttu-id="d349a-146">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="d349a-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="d349a-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="d349a-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="d349a-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="d349a-148">Boolean</span></span>|<span data-ttu-id="d349a-149">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="d349a-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="d349a-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="d349a-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="d349a-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d349a-151">Boolean</span></span>|<span data-ttu-id="d349a-152">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="d349a-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="d349a-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="d349a-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="d349a-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="d349a-154">Boolean</span></span>|<span data-ttu-id="d349a-155">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="d349a-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="d349a-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="d349a-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="d349a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="d349a-157">Int32</span></span>|<span data-ttu-id="d349a-158">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="d349a-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="d349a-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="d349a-159">Response</span></span>
<span data-ttu-id="d349a-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d349a-160">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d349a-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d349a-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="d349a-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d349a-162">Request</span></span>
<span data-ttu-id="d349a-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d349a-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d349a-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="d349a-164">Response</span></span>
<span data-ttu-id="d349a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d349a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



