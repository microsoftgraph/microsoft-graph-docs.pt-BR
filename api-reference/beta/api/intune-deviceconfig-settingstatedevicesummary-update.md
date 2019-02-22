---
title: Atualizar settingStateDeviceSummary
description: Atualizar as propriedades de um objeto settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13e8c4f61156f37a24b81cb08685215c8ae560a9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156935"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="82e92-103">Atualizar settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="82e92-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="82e92-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82e92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82e92-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82e92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82e92-106">Atualizar as propriedades de um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="82e92-106">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82e92-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82e92-107">Prerequisites</span></span>
<span data-ttu-id="82e92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="82e92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="82e92-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82e92-110">Permission type</span></span>|<span data-ttu-id="82e92-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82e92-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82e92-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82e92-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82e92-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82e92-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82e92-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82e92-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82e92-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82e92-115">Not supported.</span></span>|
|<span data-ttu-id="82e92-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82e92-116">Application</span></span>|<span data-ttu-id="82e92-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82e92-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82e92-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82e92-118">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="82e92-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82e92-119">Request headers</span></span>
|<span data-ttu-id="82e92-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82e92-120">Header</span></span>|<span data-ttu-id="82e92-121">Valor</span><span class="sxs-lookup"><span data-stu-id="82e92-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82e92-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="82e92-122">Authorization</span></span>|<span data-ttu-id="82e92-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82e92-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82e92-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82e92-124">Accept</span></span>|<span data-ttu-id="82e92-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82e92-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82e92-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82e92-126">Request body</span></span>
<span data-ttu-id="82e92-127">No corpo da solicitação, forneça uma representação JSON do objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="82e92-127">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="82e92-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="82e92-128">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="82e92-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82e92-129">Property</span></span>|<span data-ttu-id="82e92-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="82e92-130">Type</span></span>|<span data-ttu-id="82e92-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="82e92-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82e92-132">id</span><span class="sxs-lookup"><span data-stu-id="82e92-132">id</span></span>|<span data-ttu-id="82e92-133">String</span><span class="sxs-lookup"><span data-stu-id="82e92-133">String</span></span>|<span data-ttu-id="82e92-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="82e92-134">Key of the entity.</span></span>|
|<span data-ttu-id="82e92-135">settingName</span><span class="sxs-lookup"><span data-stu-id="82e92-135">settingName</span></span>|<span data-ttu-id="82e92-136">String</span><span class="sxs-lookup"><span data-stu-id="82e92-136">String</span></span>|<span data-ttu-id="82e92-137">Nome da configuração</span><span class="sxs-lookup"><span data-stu-id="82e92-137">Name of the setting</span></span>|
|<span data-ttu-id="82e92-138">instancePath</span><span class="sxs-lookup"><span data-stu-id="82e92-138">instancePath</span></span>|<span data-ttu-id="82e92-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82e92-139">String</span></span>|<span data-ttu-id="82e92-140">Nome de InstancePath para a configuração</span><span class="sxs-lookup"><span data-stu-id="82e92-140">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="82e92-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82e92-141">unknownDeviceCount</span></span>|<span data-ttu-id="82e92-142">Int32</span><span class="sxs-lookup"><span data-stu-id="82e92-142">Int32</span></span>|<span data-ttu-id="82e92-143">Contagem desconhecida de dispositivos para a configuração</span><span class="sxs-lookup"><span data-stu-id="82e92-143">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="82e92-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82e92-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="82e92-145">Int32</span><span class="sxs-lookup"><span data-stu-id="82e92-145">Int32</span></span>|<span data-ttu-id="82e92-146">Contagem não aplicável ao dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="82e92-146">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="82e92-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82e92-147">compliantDeviceCount</span></span>|<span data-ttu-id="82e92-148">Int32</span><span class="sxs-lookup"><span data-stu-id="82e92-148">Int32</span></span>|<span data-ttu-id="82e92-149">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="82e92-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="82e92-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82e92-150">remediatedDeviceCount</span></span>|<span data-ttu-id="82e92-151">Int32</span><span class="sxs-lookup"><span data-stu-id="82e92-151">Int32</span></span>|<span data-ttu-id="82e92-152">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="82e92-152">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="82e92-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82e92-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="82e92-154">Int32</span><span class="sxs-lookup"><span data-stu-id="82e92-154">Int32</span></span>|<span data-ttu-id="82e92-155">Contagem de dispositivo sem conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="82e92-155">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="82e92-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82e92-156">errorDeviceCount</span></span>|<span data-ttu-id="82e92-157">Int32</span><span class="sxs-lookup"><span data-stu-id="82e92-157">Int32</span></span>|<span data-ttu-id="82e92-158">Contagem de erros de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="82e92-158">Device error count for the setting</span></span>|
|<span data-ttu-id="82e92-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82e92-159">conflictDeviceCount</span></span>|<span data-ttu-id="82e92-160">Int32</span><span class="sxs-lookup"><span data-stu-id="82e92-160">Int32</span></span>|<span data-ttu-id="82e92-161">Contagem de erro de conflito de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="82e92-161">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="82e92-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="82e92-162">Response</span></span>
<span data-ttu-id="82e92-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82e92-163">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82e92-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82e92-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="82e92-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82e92-165">Request</span></span>
<span data-ttu-id="82e92-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82e92-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82e92-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="82e92-167">Response</span></span>
<span data-ttu-id="82e92-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82e92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




