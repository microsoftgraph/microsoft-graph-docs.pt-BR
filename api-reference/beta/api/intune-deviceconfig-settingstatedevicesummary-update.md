---
title: Atualizar settingStateDeviceSummary
description: Atualizar as propriedades de um objeto settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4745c0711d190b7b646245c3f042465e6e07bec4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43342232"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="40dd7-103">Atualizar settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="40dd7-103">Update settingStateDeviceSummary</span></span>

<span data-ttu-id="40dd7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40dd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40dd7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40dd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40dd7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40dd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40dd7-107">Atualizar as propriedades de um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="40dd7-107">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40dd7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40dd7-108">Prerequisites</span></span>
<span data-ttu-id="40dd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40dd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40dd7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40dd7-111">Permission type</span></span>|<span data-ttu-id="40dd7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40dd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40dd7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40dd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40dd7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40dd7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40dd7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40dd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40dd7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40dd7-116">Not supported.</span></span>|
|<span data-ttu-id="40dd7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40dd7-117">Application</span></span>|<span data-ttu-id="40dd7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40dd7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40dd7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40dd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="40dd7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40dd7-120">Request headers</span></span>
|<span data-ttu-id="40dd7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40dd7-121">Header</span></span>|<span data-ttu-id="40dd7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="40dd7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40dd7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="40dd7-123">Authorization</span></span>|<span data-ttu-id="40dd7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40dd7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40dd7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40dd7-125">Accept</span></span>|<span data-ttu-id="40dd7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40dd7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40dd7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40dd7-127">Request body</span></span>
<span data-ttu-id="40dd7-128">No corpo da solicitação, forneça uma representação JSON do objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="40dd7-128">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="40dd7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="40dd7-129">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="40dd7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40dd7-130">Property</span></span>|<span data-ttu-id="40dd7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="40dd7-131">Type</span></span>|<span data-ttu-id="40dd7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="40dd7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40dd7-133">id</span><span class="sxs-lookup"><span data-stu-id="40dd7-133">id</span></span>|<span data-ttu-id="40dd7-134">String</span><span class="sxs-lookup"><span data-stu-id="40dd7-134">String</span></span>|<span data-ttu-id="40dd7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="40dd7-135">Key of the entity.</span></span>|
|<span data-ttu-id="40dd7-136">settingName</span><span class="sxs-lookup"><span data-stu-id="40dd7-136">settingName</span></span>|<span data-ttu-id="40dd7-137">String</span><span class="sxs-lookup"><span data-stu-id="40dd7-137">String</span></span>|<span data-ttu-id="40dd7-138">Nome da configuração</span><span class="sxs-lookup"><span data-stu-id="40dd7-138">Name of the setting</span></span>|
|<span data-ttu-id="40dd7-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="40dd7-139">instancePath</span></span>|<span data-ttu-id="40dd7-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40dd7-140">String</span></span>|<span data-ttu-id="40dd7-141">Nome de InstancePath para a configuração</span><span class="sxs-lookup"><span data-stu-id="40dd7-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="40dd7-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40dd7-142">unknownDeviceCount</span></span>|<span data-ttu-id="40dd7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="40dd7-143">Int32</span></span>|<span data-ttu-id="40dd7-144">Contagem desconhecida de dispositivos para a configuração</span><span class="sxs-lookup"><span data-stu-id="40dd7-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="40dd7-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40dd7-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="40dd7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="40dd7-146">Int32</span></span>|<span data-ttu-id="40dd7-147">Contagem não aplicável ao dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="40dd7-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="40dd7-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40dd7-148">compliantDeviceCount</span></span>|<span data-ttu-id="40dd7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="40dd7-149">Int32</span></span>|<span data-ttu-id="40dd7-150">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="40dd7-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="40dd7-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40dd7-151">remediatedDeviceCount</span></span>|<span data-ttu-id="40dd7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="40dd7-152">Int32</span></span>|<span data-ttu-id="40dd7-153">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="40dd7-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="40dd7-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40dd7-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="40dd7-155">Int32</span><span class="sxs-lookup"><span data-stu-id="40dd7-155">Int32</span></span>|<span data-ttu-id="40dd7-156">Contagem de dispositivo sem conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="40dd7-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="40dd7-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40dd7-157">errorDeviceCount</span></span>|<span data-ttu-id="40dd7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="40dd7-158">Int32</span></span>|<span data-ttu-id="40dd7-159">Contagem de erros de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="40dd7-159">Device error count for the setting</span></span>|
|<span data-ttu-id="40dd7-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="40dd7-160">conflictDeviceCount</span></span>|<span data-ttu-id="40dd7-161">Int32</span><span class="sxs-lookup"><span data-stu-id="40dd7-161">Int32</span></span>|<span data-ttu-id="40dd7-162">Contagem de erro de conflito de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="40dd7-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="40dd7-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="40dd7-163">Response</span></span>
<span data-ttu-id="40dd7-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40dd7-164">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40dd7-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40dd7-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="40dd7-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40dd7-166">Request</span></span>
<span data-ttu-id="40dd7-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40dd7-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="40dd7-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="40dd7-168">Response</span></span>
<span data-ttu-id="40dd7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40dd7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



