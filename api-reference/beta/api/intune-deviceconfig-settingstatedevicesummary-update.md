---
title: Atualizar settingStateDeviceSummary
description: Atualizar as propriedades de um objeto settingStateDeviceSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 93b130224cb74899d8191d576d2acf2508001a7d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127869"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="d8b70-103">Atualizar settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="d8b70-103">Update settingStateDeviceSummary</span></span>

<span data-ttu-id="d8b70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8b70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8b70-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8b70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8b70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8b70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8b70-107">Atualizar as propriedades de um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d8b70-107">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8b70-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8b70-108">Prerequisites</span></span>
<span data-ttu-id="d8b70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8b70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8b70-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8b70-111">Permission type</span></span>|<span data-ttu-id="d8b70-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8b70-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8b70-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8b70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8b70-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8b70-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8b70-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8b70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8b70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8b70-116">Not supported.</span></span>|
|<span data-ttu-id="d8b70-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8b70-117">Application</span></span>|<span data-ttu-id="d8b70-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8b70-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8b70-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8b70-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d8b70-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8b70-120">Request headers</span></span>
|<span data-ttu-id="d8b70-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8b70-121">Header</span></span>|<span data-ttu-id="d8b70-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d8b70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8b70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8b70-123">Authorization</span></span>|<span data-ttu-id="d8b70-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8b70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8b70-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8b70-125">Accept</span></span>|<span data-ttu-id="d8b70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8b70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8b70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8b70-127">Request body</span></span>
<span data-ttu-id="d8b70-128">No corpo da solicitação, forneça uma representação JSON do objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d8b70-128">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="d8b70-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="d8b70-129">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="d8b70-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8b70-130">Property</span></span>|<span data-ttu-id="d8b70-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8b70-131">Type</span></span>|<span data-ttu-id="d8b70-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8b70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8b70-133">id</span><span class="sxs-lookup"><span data-stu-id="d8b70-133">id</span></span>|<span data-ttu-id="d8b70-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8b70-134">String</span></span>|<span data-ttu-id="d8b70-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d8b70-135">Key of the entity.</span></span>|
|<span data-ttu-id="d8b70-136">settingName</span><span class="sxs-lookup"><span data-stu-id="d8b70-136">settingName</span></span>|<span data-ttu-id="d8b70-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8b70-137">String</span></span>|<span data-ttu-id="d8b70-138">Nome da configuração</span><span class="sxs-lookup"><span data-stu-id="d8b70-138">Name of the setting</span></span>|
|<span data-ttu-id="d8b70-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="d8b70-139">instancePath</span></span>|<span data-ttu-id="d8b70-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8b70-140">String</span></span>|<span data-ttu-id="d8b70-141">Nome de InstancePath para a configuração</span><span class="sxs-lookup"><span data-stu-id="d8b70-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="d8b70-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8b70-142">unknownDeviceCount</span></span>|<span data-ttu-id="d8b70-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d8b70-143">Int32</span></span>|<span data-ttu-id="d8b70-144">Contagem desconhecida de dispositivos para a configuração</span><span class="sxs-lookup"><span data-stu-id="d8b70-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="d8b70-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8b70-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="d8b70-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d8b70-146">Int32</span></span>|<span data-ttu-id="d8b70-147">Contagem não aplicável ao dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="d8b70-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="d8b70-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8b70-148">compliantDeviceCount</span></span>|<span data-ttu-id="d8b70-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d8b70-149">Int32</span></span>|<span data-ttu-id="d8b70-150">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="d8b70-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="d8b70-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8b70-151">remediatedDeviceCount</span></span>|<span data-ttu-id="d8b70-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d8b70-152">Int32</span></span>|<span data-ttu-id="d8b70-153">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="d8b70-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="d8b70-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8b70-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d8b70-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d8b70-155">Int32</span></span>|<span data-ttu-id="d8b70-156">Contagem de dispositivo sem conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="d8b70-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="d8b70-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8b70-157">errorDeviceCount</span></span>|<span data-ttu-id="d8b70-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d8b70-158">Int32</span></span>|<span data-ttu-id="d8b70-159">Contagem de erros de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="d8b70-159">Device error count for the setting</span></span>|
|<span data-ttu-id="d8b70-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d8b70-160">conflictDeviceCount</span></span>|<span data-ttu-id="d8b70-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d8b70-161">Int32</span></span>|<span data-ttu-id="d8b70-162">Contagem de erro de conflito de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="d8b70-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="d8b70-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8b70-163">Response</span></span>
<span data-ttu-id="d8b70-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8b70-164">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8b70-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8b70-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8b70-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8b70-166">Request</span></span>
<span data-ttu-id="d8b70-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8b70-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d8b70-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8b70-168">Response</span></span>
<span data-ttu-id="d8b70-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8b70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




