---
title: Atualizar windowsProtectionState
description: Atualize as propriedades de um objeto windowsProtectionState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: faad744f1a7910b693ea7f87ea0e2ab5dddd7a25
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406203"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="a0c09-103">Atualizar windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="a0c09-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="a0c09-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a0c09-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a0c09-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a0c09-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0c09-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a0c09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0c09-107">Atualize as propriedades de um objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="a0c09-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0c09-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0c09-108">Prerequisites</span></span>
<span data-ttu-id="a0c09-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a0c09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a0c09-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0c09-111">Permission type</span></span>|<span data-ttu-id="a0c09-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0c09-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0c09-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0c09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0c09-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0c09-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a0c09-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0c09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0c09-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0c09-116">Not supported.</span></span>|
|<span data-ttu-id="a0c09-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0c09-117">Application</span></span>|<span data-ttu-id="a0c09-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0c09-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0c09-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0c09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="a0c09-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0c09-120">Request headers</span></span>
|<span data-ttu-id="a0c09-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0c09-121">Header</span></span>|<span data-ttu-id="a0c09-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0c09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0c09-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0c09-123">Authorization</span></span>|<span data-ttu-id="a0c09-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0c09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0c09-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0c09-125">Accept</span></span>|<span data-ttu-id="a0c09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0c09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0c09-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0c09-127">Request body</span></span>
<span data-ttu-id="a0c09-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="a0c09-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="a0c09-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="a0c09-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="a0c09-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0c09-130">Property</span></span>|<span data-ttu-id="a0c09-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0c09-131">Type</span></span>|<span data-ttu-id="a0c09-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0c09-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0c09-133">id</span><span class="sxs-lookup"><span data-stu-id="a0c09-133">id</span></span>|<span data-ttu-id="a0c09-134">String</span><span class="sxs-lookup"><span data-stu-id="a0c09-134">String</span></span>|<span data-ttu-id="a0c09-135">O identificador exclusivo para o objeto de status de proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0c09-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="a0c09-136">Este é o id do dispositivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a0c09-136">This is device id of the device</span></span>|
|<span data-ttu-id="a0c09-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a0c09-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="a0c09-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0c09-138">Boolean</span></span>|<span data-ttu-id="a0c09-139">Anti-malware está habilitado ou não</span><span class="sxs-lookup"><span data-stu-id="a0c09-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="a0c09-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="a0c09-140">deviceState</span></span>|[<span data-ttu-id="a0c09-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="a0c09-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="a0c09-142">Estado do computador (como limpar ou verificação completa ou pendentes reinicialização etc.).</span><span class="sxs-lookup"><span data-stu-id="a0c09-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="a0c09-143">Os possíveis valores são: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="a0c09-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="a0c09-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a0c09-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="a0c09-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0c09-145">Boolean</span></span>|<span data-ttu-id="a0c09-146">Proteção em tempo real está habilitada ou não?</span><span class="sxs-lookup"><span data-stu-id="a0c09-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="a0c09-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="a0c09-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="a0c09-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0c09-148">Boolean</span></span>|<span data-ttu-id="a0c09-149">Sistema de inspeção de rede habilitado ou não?</span><span class="sxs-lookup"><span data-stu-id="a0c09-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="a0c09-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="a0c09-150">quickScanOverdue</span></span>|<span data-ttu-id="a0c09-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0c09-151">Boolean</span></span>|<span data-ttu-id="a0c09-152">Verificação rápida vencidos ou não?</span><span class="sxs-lookup"><span data-stu-id="a0c09-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="a0c09-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="a0c09-153">fullScanOverdue</span></span>|<span data-ttu-id="a0c09-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0c09-154">Boolean</span></span>|<span data-ttu-id="a0c09-155">Completos exame vencido ou não?</span><span class="sxs-lookup"><span data-stu-id="a0c09-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="a0c09-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="a0c09-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="a0c09-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0c09-157">Boolean</span></span>|<span data-ttu-id="a0c09-158">Assinatura desatualizada ou não?</span><span class="sxs-lookup"><span data-stu-id="a0c09-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="a0c09-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="a0c09-159">rebootRequired</span></span>|<span data-ttu-id="a0c09-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0c09-160">Boolean</span></span>|<span data-ttu-id="a0c09-161">Reinicialização necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="a0c09-161">Reboot required or not?</span></span>|
|<span data-ttu-id="a0c09-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="a0c09-162">fullScanRequired</span></span>|<span data-ttu-id="a0c09-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0c09-163">Boolean</span></span>|<span data-ttu-id="a0c09-164">Verificação completa necessária ou não?</span><span class="sxs-lookup"><span data-stu-id="a0c09-164">Full scan required or not?</span></span>|
|<span data-ttu-id="a0c09-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="a0c09-165">engineVersion</span></span>|<span data-ttu-id="a0c09-166">String</span><span class="sxs-lookup"><span data-stu-id="a0c09-166">String</span></span>|<span data-ttu-id="a0c09-167">Versão do mecanismo de proteção de ponto de extremidade atual</span><span class="sxs-lookup"><span data-stu-id="a0c09-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="a0c09-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="a0c09-168">signatureVersion</span></span>|<span data-ttu-id="a0c09-169">String</span><span class="sxs-lookup"><span data-stu-id="a0c09-169">String</span></span>|<span data-ttu-id="a0c09-170">Versão atual de definições de malware</span><span class="sxs-lookup"><span data-stu-id="a0c09-170">Current malware definitions version</span></span>|
|<span data-ttu-id="a0c09-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="a0c09-171">antiMalwareVersion</span></span>|<span data-ttu-id="a0c09-172">String</span><span class="sxs-lookup"><span data-stu-id="a0c09-172">String</span></span>|<span data-ttu-id="a0c09-173">Atual anti-malware versão</span><span class="sxs-lookup"><span data-stu-id="a0c09-173">Current anti malware version</span></span>|
|<span data-ttu-id="a0c09-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a0c09-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="a0c09-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0c09-175">DateTimeOffset</span></span>|<span data-ttu-id="a0c09-176">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="a0c09-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="a0c09-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a0c09-177">lastFullScanDateTime</span></span>|<span data-ttu-id="a0c09-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0c09-178">DateTimeOffset</span></span>|<span data-ttu-id="a0c09-179">Última data/hora de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="a0c09-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="a0c09-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a0c09-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="a0c09-181">String</span><span class="sxs-lookup"><span data-stu-id="a0c09-181">String</span></span>|<span data-ttu-id="a0c09-182">Última versão de assinatura de verificação rápida</span><span class="sxs-lookup"><span data-stu-id="a0c09-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="a0c09-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a0c09-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="a0c09-184">String</span><span class="sxs-lookup"><span data-stu-id="a0c09-184">String</span></span>|<span data-ttu-id="a0c09-185">Última versão de assinatura de verificação completa</span><span class="sxs-lookup"><span data-stu-id="a0c09-185">Last full scan signature version</span></span>|
|<span data-ttu-id="a0c09-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0c09-186">lastReportedDateTime</span></span>|<span data-ttu-id="a0c09-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0c09-187">DateTimeOffset</span></span>|<span data-ttu-id="a0c09-188">Tempo de informado último status de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a0c09-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="a0c09-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0c09-189">Response</span></span>
<span data-ttu-id="a0c09-190">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0c09-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0c09-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0c09-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0c09-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0c09-192">Request</span></span>
<span data-ttu-id="a0c09-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0c09-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 865

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="a0c09-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0c09-194">Response</span></span>
<span data-ttu-id="a0c09-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0c09-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```




