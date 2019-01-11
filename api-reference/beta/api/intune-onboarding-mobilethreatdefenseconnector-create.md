---
title: Criar mobileThreatDefenseConnector
description: Cria um novo objeto mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a1ead3e352723e8dc345c94eee513c8fb0c1aaa7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854891"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="1ae7d-103">Criar mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="1ae7d-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="1ae7d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ae7d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ae7d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ae7d-107">Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="1ae7d-107">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ae7d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ae7d-108">Prerequisites</span></span>
<span data-ttu-id="1ae7d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ae7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ae7d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ae7d-111">Permission type</span></span>|<span data-ttu-id="1ae7d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ae7d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ae7d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ae7d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ae7d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ae7d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1ae7d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ae7d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ae7d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-116">Not supported.</span></span>|
|<span data-ttu-id="1ae7d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ae7d-117">Application</span></span>|<span data-ttu-id="1ae7d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ae7d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ae7d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="1ae7d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ae7d-120">Request headers</span></span>
|<span data-ttu-id="1ae7d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ae7d-121">Header</span></span>|<span data-ttu-id="1ae7d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1ae7d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ae7d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ae7d-123">Authorization</span></span>|<span data-ttu-id="1ae7d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ae7d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ae7d-125">Accept</span></span>|<span data-ttu-id="1ae7d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ae7d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ae7d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ae7d-127">Request body</span></span>
<span data-ttu-id="1ae7d-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-128">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="1ae7d-129">A tabela a seguir mostra as propriedades obrigatórias ao criar mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-129">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="1ae7d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ae7d-130">Property</span></span>|<span data-ttu-id="1ae7d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ae7d-131">Type</span></span>|<span data-ttu-id="1ae7d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ae7d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ae7d-133">id</span><span class="sxs-lookup"><span data-stu-id="1ae7d-133">id</span></span>|<span data-ttu-id="1ae7d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ae7d-134">String</span></span>|<span data-ttu-id="1ae7d-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1ae7d-135">Not yet documented</span></span>|
|<span data-ttu-id="1ae7d-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="1ae7d-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="1ae7d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ae7d-137">DateTimeOffset</span></span>|<span data-ttu-id="1ae7d-138">Data e hora da última Pulsação recebida de um Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="1ae7d-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="1ae7d-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="1ae7d-139">partnerState</span></span>|[<span data-ttu-id="1ae7d-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="1ae7d-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="1ae7d-141">Estado de parceiro de sincronização de dados para essa conta.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="1ae7d-142">Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="1ae7d-143">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="1ae7d-143">androidEnabled</span></span>|<span data-ttu-id="1ae7d-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ae7d-144">Boolean</span></span>|<span data-ttu-id="1ae7d-145">No Android, definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="1ae7d-145">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="1ae7d-146">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="1ae7d-146">iosEnabled</span></span>|<span data-ttu-id="1ae7d-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ae7d-147">Boolean</span></span>|<span data-ttu-id="1ae7d-148">No iOS, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="1ae7d-148">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="1ae7d-149">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="1ae7d-149">windowsEnabled</span></span>|<span data-ttu-id="1ae7d-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="1ae7d-150">Boolean</span></span>|<span data-ttu-id="1ae7d-151">Para Windows, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="1ae7d-151">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="1ae7d-152">macEnabled</span><span class="sxs-lookup"><span data-stu-id="1ae7d-152">macEnabled</span></span>|<span data-ttu-id="1ae7d-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="1ae7d-153">Boolean</span></span>|<span data-ttu-id="1ae7d-154">Para Mac, obter ou definir se os dados do parceiro de sincronização de dados devem ser usados durante as avaliações de conformidade</span><span class="sxs-lookup"><span data-stu-id="1ae7d-154">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="1ae7d-155">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="1ae7d-155">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="1ae7d-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ae7d-156">Boolean</span></span>|<span data-ttu-id="1ae7d-157">No Android, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="1ae7d-157">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="1ae7d-158">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="1ae7d-158">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="1ae7d-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ae7d-159">Boolean</span></span>|<span data-ttu-id="1ae7d-160">No iOS, definir se o Intune deve receber os dados do parceiro de sincronização de dados antes de marcar um dispositivo como compatível</span><span class="sxs-lookup"><span data-stu-id="1ae7d-160">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="1ae7d-161">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="1ae7d-161">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="1ae7d-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="1ae7d-162">Boolean</span></span>|<span data-ttu-id="1ae7d-163">Para Windows, defina se Intune deve receber dados do parceiro de sincronização de dados antes da marcação de um dispositivo compatível com</span><span class="sxs-lookup"><span data-stu-id="1ae7d-163">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="1ae7d-164">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="1ae7d-164">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="1ae7d-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="1ae7d-165">Boolean</span></span>|<span data-ttu-id="1ae7d-166">Para Mac, obter ou definir se Intune deve receber dados do parceiro de sincronização de dados antes da marcação de um dispositivo compatível com</span><span class="sxs-lookup"><span data-stu-id="1ae7d-166">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="1ae7d-167">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="1ae7d-167">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="1ae7d-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ae7d-168">Boolean</span></span>|<span data-ttu-id="1ae7d-169">Obter ou definir se dispositivos devem ser bloqueados nas plataformas habilitadas que não atendam aos requisitos mínimos de versão do Parceiro de Sincronização de Dados</span><span class="sxs-lookup"><span data-stu-id="1ae7d-169">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="1ae7d-170">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="1ae7d-170">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="1ae7d-171">Int32</span><span class="sxs-lookup"><span data-stu-id="1ae7d-171">Int32</span></span>|<span data-ttu-id="1ae7d-172">Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro</span><span class="sxs-lookup"><span data-stu-id="1ae7d-172">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="1ae7d-173">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="1ae7d-173">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="1ae7d-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="1ae7d-174">Boolean</span></span>|<span data-ttu-id="1ae7d-175">Para dispositivos IOS, permite que o administrador configurar se o parceiro de sincronização de dados também pode coletar metadados sobre os aplicativos instalados de Intune</span><span class="sxs-lookup"><span data-stu-id="1ae7d-175">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="1ae7d-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ae7d-176">Response</span></span>
<span data-ttu-id="1ae7d-177">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-177">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ae7d-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ae7d-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ae7d-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ae7d-179">Request</span></span>
<span data-ttu-id="1ae7d-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 622

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
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

### <a name="response"></a><span data-ttu-id="1ae7d-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ae7d-181">Response</span></span>
<span data-ttu-id="1ae7d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ae7d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





