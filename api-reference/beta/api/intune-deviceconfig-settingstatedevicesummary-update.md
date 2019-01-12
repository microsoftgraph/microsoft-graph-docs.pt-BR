---
title: Atualizar settingStateDeviceSummary
description: Atualizar as propriedades de um objeto settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ab0a3ec4609ce3f5015d9bb1ae6f1b815f5d6b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920594"
---
# <a name="update-settingstatedevicesummary"></a><span data-ttu-id="72567-103">Atualizar settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="72567-103">Update settingStateDeviceSummary</span></span>

> <span data-ttu-id="72567-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="72567-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72567-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="72567-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72567-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="72567-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72567-107">Atualizar as propriedades de um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="72567-107">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72567-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72567-108">Prerequisites</span></span>
<span data-ttu-id="72567-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72567-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72567-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72567-111">Permission type</span></span>|<span data-ttu-id="72567-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72567-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72567-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72567-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72567-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72567-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72567-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72567-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72567-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72567-116">Not supported.</span></span>|
|<span data-ttu-id="72567-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72567-117">Application</span></span>|<span data-ttu-id="72567-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72567-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72567-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72567-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="72567-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72567-120">Request headers</span></span>
|<span data-ttu-id="72567-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72567-121">Header</span></span>|<span data-ttu-id="72567-122">Valor</span><span class="sxs-lookup"><span data-stu-id="72567-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72567-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="72567-123">Authorization</span></span>|<span data-ttu-id="72567-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72567-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72567-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72567-125">Accept</span></span>|<span data-ttu-id="72567-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72567-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72567-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72567-127">Request body</span></span>
<span data-ttu-id="72567-128">No corpo da solicitação, forneça uma representação JSON do objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="72567-128">In the request body, supply a JSON representation for the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

<span data-ttu-id="72567-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="72567-129">The following table shows the properties that are required when you create the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>

|<span data-ttu-id="72567-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72567-130">Property</span></span>|<span data-ttu-id="72567-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="72567-131">Type</span></span>|<span data-ttu-id="72567-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="72567-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72567-133">id</span><span class="sxs-lookup"><span data-stu-id="72567-133">id</span></span>|<span data-ttu-id="72567-134">String</span><span class="sxs-lookup"><span data-stu-id="72567-134">String</span></span>|<span data-ttu-id="72567-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="72567-135">Key of the entity.</span></span>|
|<span data-ttu-id="72567-136">settingName</span><span class="sxs-lookup"><span data-stu-id="72567-136">settingName</span></span>|<span data-ttu-id="72567-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72567-137">String</span></span>|<span data-ttu-id="72567-138">Nome da configuração</span><span class="sxs-lookup"><span data-stu-id="72567-138">Name of the setting</span></span>|
|<span data-ttu-id="72567-139">instancePath</span><span class="sxs-lookup"><span data-stu-id="72567-139">instancePath</span></span>|<span data-ttu-id="72567-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72567-140">String</span></span>|<span data-ttu-id="72567-141">Nome de InstancePath para a configuração</span><span class="sxs-lookup"><span data-stu-id="72567-141">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="72567-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72567-142">unknownDeviceCount</span></span>|<span data-ttu-id="72567-143">Int32</span><span class="sxs-lookup"><span data-stu-id="72567-143">Int32</span></span>|<span data-ttu-id="72567-144">Contagem desconhecida de dispositivos para a configuração</span><span class="sxs-lookup"><span data-stu-id="72567-144">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="72567-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72567-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="72567-146">Int32</span><span class="sxs-lookup"><span data-stu-id="72567-146">Int32</span></span>|<span data-ttu-id="72567-147">Contagem não aplicável ao dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="72567-147">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="72567-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72567-148">compliantDeviceCount</span></span>|<span data-ttu-id="72567-149">Int32</span><span class="sxs-lookup"><span data-stu-id="72567-149">Int32</span></span>|<span data-ttu-id="72567-150">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="72567-150">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="72567-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72567-151">remediatedDeviceCount</span></span>|<span data-ttu-id="72567-152">Int32</span><span class="sxs-lookup"><span data-stu-id="72567-152">Int32</span></span>|<span data-ttu-id="72567-153">Contagem de dispositivo em conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="72567-153">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="72567-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72567-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="72567-155">Int32</span><span class="sxs-lookup"><span data-stu-id="72567-155">Int32</span></span>|<span data-ttu-id="72567-156">Contagem de dispositivo sem conformidade para a configuração</span><span class="sxs-lookup"><span data-stu-id="72567-156">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="72567-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72567-157">errorDeviceCount</span></span>|<span data-ttu-id="72567-158">Int32</span><span class="sxs-lookup"><span data-stu-id="72567-158">Int32</span></span>|<span data-ttu-id="72567-159">Contagem de erros de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="72567-159">Device error count for the setting</span></span>|
|<span data-ttu-id="72567-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72567-160">conflictDeviceCount</span></span>|<span data-ttu-id="72567-161">Int32</span><span class="sxs-lookup"><span data-stu-id="72567-161">Int32</span></span>|<span data-ttu-id="72567-162">Contagem de erro de conflito de dispositivo para a configuração</span><span class="sxs-lookup"><span data-stu-id="72567-162">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="72567-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="72567-163">Response</span></span>
<span data-ttu-id="72567-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72567-164">If successful, this method returns a `200 OK` response code and an updated [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72567-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72567-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="72567-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72567-166">Request</span></span>
<span data-ttu-id="72567-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72567-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
Content-type: application/json
Content-length: 296

{
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

### <a name="response"></a><span data-ttu-id="72567-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="72567-168">Response</span></span>
<span data-ttu-id="72567-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72567-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





