---
title: Atualizar mobileThreatDefenseConnector
description: Atualiza as propriedades de um objeto mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2d256ac641d403d12417de9afcbfb473d9bfe944
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865664"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="5dfe5-103">Atualizar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="5dfe5-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="5dfe5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5dfe5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5dfe5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5dfe5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5dfe5-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5dfe5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5dfe5-107">Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="5dfe5-107">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5dfe5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5dfe5-108">Prerequisites</span></span>
<span data-ttu-id="5dfe5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dfe5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dfe5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dfe5-111">Permission type</span></span>|<span data-ttu-id="5dfe5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5dfe5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dfe5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dfe5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5dfe5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dfe5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5dfe5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dfe5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dfe5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dfe5-116">Not supported.</span></span>|
|<span data-ttu-id="5dfe5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dfe5-117">Application</span></span>|<span data-ttu-id="5dfe5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dfe5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dfe5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dfe5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="5dfe5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dfe5-120">Request headers</span></span>
|<span data-ttu-id="5dfe5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5dfe5-121">Header</span></span>|<span data-ttu-id="5dfe5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5dfe5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dfe5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dfe5-123">Authorization</span></span>|<span data-ttu-id="5dfe5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dfe5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dfe5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5dfe5-125">Accept</span></span>|<span data-ttu-id="5dfe5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5dfe5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dfe5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dfe5-127">Request body</span></span>
<span data-ttu-id="5dfe5-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="5dfe5-128">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="5dfe5-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="5dfe5-129">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="5dfe5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dfe5-130">Property</span></span>|<span data-ttu-id="5dfe5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dfe5-131">Type</span></span>|<span data-ttu-id="5dfe5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dfe5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dfe5-133">id</span><span class="sxs-lookup"><span data-stu-id="5dfe5-133">id</span></span>|<span data-ttu-id="5dfe5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dfe5-134">String</span></span>|<span data-ttu-id="5dfe5-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5dfe5-135">Not yet documented</span></span>|
|<span data-ttu-id="5dfe5-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="5dfe5-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="5dfe5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dfe5-137">DateTimeOffset</span></span>|<span data-ttu-id="5dfe5-138">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="5dfe5-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="5dfe5-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="5dfe5-139">partnerState</span></span>|[<span data-ttu-id="5dfe5-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="5dfe5-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="5dfe5-141">Estado de parceiro de sincronização de dados para essa conta.</span><span class="sxs-lookup"><span data-stu-id="5dfe5-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="5dfe5-142">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="5dfe5-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="5dfe5-143">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="5dfe5-143">androidEnabled</span></span>|<span data-ttu-id="5dfe5-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfe5-144">Boolean</span></span>|<span data-ttu-id="5dfe5-145">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="5dfe5-145">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="5dfe5-146">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="5dfe5-146">iosEnabled</span></span>|<span data-ttu-id="5dfe5-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfe5-147">Boolean</span></span>|<span data-ttu-id="5dfe5-148">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="5dfe5-148">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="5dfe5-149">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="5dfe5-149">windowsEnabled</span></span>|<span data-ttu-id="5dfe5-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="5dfe5-150">Boolean</span></span>|<span data-ttu-id="5dfe5-151">Para Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="5dfe5-151">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="5dfe5-152">macEnabled</span><span class="sxs-lookup"><span data-stu-id="5dfe5-152">macEnabled</span></span>|<span data-ttu-id="5dfe5-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="5dfe5-153">Boolean</span></span>|<span data-ttu-id="5dfe5-154">Para Mac, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="5dfe5-154">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="5dfe5-155">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="5dfe5-155">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="5dfe5-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfe5-156">Boolean</span></span>|<span data-ttu-id="5dfe5-157">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="5dfe5-157">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="5dfe5-158">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="5dfe5-158">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="5dfe5-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfe5-159">Boolean</span></span>|<span data-ttu-id="5dfe5-160">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="5dfe5-160">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="5dfe5-161">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="5dfe5-161">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="5dfe5-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="5dfe5-162">Boolean</span></span>|<span data-ttu-id="5dfe5-163">Para Windows, defina se Intune deve receber dados do parceiro de sincronização de dados antes da marcação de um dispositivo compatível com</span><span class="sxs-lookup"><span data-stu-id="5dfe5-163">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="5dfe5-164">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="5dfe5-164">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="5dfe5-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="5dfe5-165">Boolean</span></span>|<span data-ttu-id="5dfe5-166">Para Mac, obter ou definir se Intune deve receber dados do parceiro de sincronização de dados antes da marcação de um dispositivo compatível com</span><span class="sxs-lookup"><span data-stu-id="5dfe5-166">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="5dfe5-167">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="5dfe5-167">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="5dfe5-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfe5-168">Boolean</span></span>|<span data-ttu-id="5dfe5-169">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="5dfe5-169">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="5dfe5-170">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="5dfe5-170">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="5dfe5-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5dfe5-171">Int32</span></span>|<span data-ttu-id="5dfe5-172">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="5dfe5-172">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="5dfe5-173">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="5dfe5-173">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="5dfe5-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="5dfe5-174">Boolean</span></span>|<span data-ttu-id="5dfe5-175">Para dispositivos IOS, permite que o administrador configurar se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados de Intune</span><span class="sxs-lookup"><span data-stu-id="5dfe5-175">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="5dfe5-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dfe5-176">Response</span></span>
<span data-ttu-id="5dfe5-177">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dfe5-177">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dfe5-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dfe5-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="5dfe5-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dfe5-179">Request</span></span>
<span data-ttu-id="5dfe5-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dfe5-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 555

{
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

### <a name="response"></a><span data-ttu-id="5dfe5-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dfe5-181">Response</span></span>
<span data-ttu-id="5dfe5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dfe5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





