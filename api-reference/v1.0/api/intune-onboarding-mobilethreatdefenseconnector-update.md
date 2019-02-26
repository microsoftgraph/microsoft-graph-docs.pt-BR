---
title: Atualizar mobileThreatDefenseConnector
description: Atualiza as propriedades de um objeto mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71d72ca72e3eba2522881081d0b44804a33fd803
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262304"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="019b7-103">Atualizar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="019b7-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="019b7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="019b7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="019b7-105">Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-105">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="019b7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="019b7-106">Prerequisites</span></span>
<span data-ttu-id="019b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="019b7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="019b7-109">Permission type</span></span>|<span data-ttu-id="019b7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="019b7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="019b7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="019b7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="019b7-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="019b7-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="019b7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="019b7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="019b7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="019b7-114">Not supported.</span></span>|
|<span data-ttu-id="019b7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="019b7-115">Application</span></span>|<span data-ttu-id="019b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="019b7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="019b7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="019b7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="019b7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="019b7-118">Request headers</span></span>
|<span data-ttu-id="019b7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="019b7-119">Header</span></span>|<span data-ttu-id="019b7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="019b7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="019b7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="019b7-121">Authorization</span></span>|<span data-ttu-id="019b7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="019b7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="019b7-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="019b7-123">Accept</span></span>|<span data-ttu-id="019b7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="019b7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="019b7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="019b7-125">Request body</span></span>
<span data-ttu-id="019b7-126">No corpo da solicitação, forneça uma representação JSON do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-126">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="019b7-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="019b7-127">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="019b7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="019b7-128">Property</span></span>|<span data-ttu-id="019b7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="019b7-129">Type</span></span>|<span data-ttu-id="019b7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="019b7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="019b7-131">id</span><span class="sxs-lookup"><span data-stu-id="019b7-131">id</span></span>|<span data-ttu-id="019b7-132">String</span><span class="sxs-lookup"><span data-stu-id="019b7-132">String</span></span>|<span data-ttu-id="019b7-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="019b7-133">Not yet documented</span></span>|
|<span data-ttu-id="019b7-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="019b7-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="019b7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="019b7-135">DateTimeOffset</span></span>|<span data-ttu-id="019b7-136">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="019b7-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="019b7-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="019b7-137">partnerState</span></span>|[<span data-ttu-id="019b7-138">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="019b7-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="019b7-139">Estado do parceiro de sincronização de dados para esta conta.</span><span class="sxs-lookup"><span data-stu-id="019b7-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="019b7-140">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="019b7-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="019b7-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="019b7-141">androidEnabled</span></span>|<span data-ttu-id="019b7-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="019b7-142">Boolean</span></span>|<span data-ttu-id="019b7-143">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="019b7-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="019b7-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="019b7-144">iosEnabled</span></span>|<span data-ttu-id="019b7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="019b7-145">Boolean</span></span>|<span data-ttu-id="019b7-146">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="019b7-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="019b7-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="019b7-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="019b7-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="019b7-148">Boolean</span></span>|<span data-ttu-id="019b7-149">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="019b7-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="019b7-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="019b7-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="019b7-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="019b7-151">Boolean</span></span>|<span data-ttu-id="019b7-152">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="019b7-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="019b7-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="019b7-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="019b7-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="019b7-154">Boolean</span></span>|<span data-ttu-id="019b7-155">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="019b7-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="019b7-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="019b7-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="019b7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="019b7-157">Int32</span></span>|<span data-ttu-id="019b7-158">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="019b7-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="019b7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="019b7-159">Response</span></span>
<span data-ttu-id="019b7-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="019b7-160">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="019b7-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="019b7-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="019b7-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="019b7-162">Request</span></span>
<span data-ttu-id="019b7-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="019b7-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="019b7-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="019b7-164">Response</span></span>
<span data-ttu-id="019b7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="019b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



