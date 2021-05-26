---
title: Atualizar deviceManagementConfigurationSettingTemplate
description: Atualize as propriedades de um objeto deviceManagementConfigurationSettingTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 98cd26899ec0b2661635dc0758997ecb876cf7d3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664818"
---
# <a name="update-devicemanagementconfigurationsettingtemplate"></a><span data-ttu-id="64a6b-103">Atualizar deviceManagementConfigurationSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="64a6b-103">Update deviceManagementConfigurationSettingTemplate</span></span>

<span data-ttu-id="64a6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64a6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64a6b-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64a6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64a6b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64a6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64a6b-107">Atualize as propriedades de [um objeto deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="64a6b-107">Update the properties of a [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64a6b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="64a6b-108">Prerequisites</span></span>
<span data-ttu-id="64a6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64a6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64a6b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64a6b-111">Permission type</span></span>|<span data-ttu-id="64a6b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64a6b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64a6b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64a6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64a6b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64a6b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64a6b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64a6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64a6b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64a6b-116">Not supported.</span></span>|
|<span data-ttu-id="64a6b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64a6b-117">Application</span></span>|<span data-ttu-id="64a6b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64a6b-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64a6b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64a6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templateSettings/{deviceManagementConfigurationSettingTemplateId}
PATCH /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="64a6b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64a6b-120">Request headers</span></span>
|<span data-ttu-id="64a6b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="64a6b-121">Header</span></span>|<span data-ttu-id="64a6b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="64a6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64a6b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="64a6b-123">Authorization</span></span>|<span data-ttu-id="64a6b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64a6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64a6b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="64a6b-125">Accept</span></span>|<span data-ttu-id="64a6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64a6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64a6b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64a6b-127">Request body</span></span>
<span data-ttu-id="64a6b-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="64a6b-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object.</span></span>

<span data-ttu-id="64a6b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="64a6b-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md).</span></span>

|<span data-ttu-id="64a6b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64a6b-130">Property</span></span>|<span data-ttu-id="64a6b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="64a6b-131">Type</span></span>|<span data-ttu-id="64a6b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="64a6b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64a6b-133">id</span><span class="sxs-lookup"><span data-stu-id="64a6b-133">id</span></span>|<span data-ttu-id="64a6b-134">String</span><span class="sxs-lookup"><span data-stu-id="64a6b-134">String</span></span>|<span data-ttu-id="64a6b-135">Chave deste modelo de configuração no modelo de política que o contém.</span><span class="sxs-lookup"><span data-stu-id="64a6b-135">Key of this setting template within the policy template which contains it.</span></span> <span data-ttu-id="64a6b-136">Gerado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="64a6b-136">Automatically generated.</span></span>|
|<span data-ttu-id="64a6b-137">settingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="64a6b-137">settingInstanceTemplate</span></span>|[<span data-ttu-id="64a6b-138">deviceManagementConfigurationSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="64a6b-138">deviceManagementConfigurationSettingInstanceTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|<span data-ttu-id="64a6b-139">Modelo de instância de configuração</span><span class="sxs-lookup"><span data-stu-id="64a6b-139">Setting Instance Template</span></span>|



## <a name="response"></a><span data-ttu-id="64a6b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="64a6b-140">Response</span></span>
<span data-ttu-id="64a6b-141">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64a6b-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64a6b-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64a6b-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="64a6b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64a6b-143">Request</span></span>
<span data-ttu-id="64a6b-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64a6b-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templateSettings/{deviceManagementConfigurationSettingTemplateId}
Content-type: application/json
Content-length: 784

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingTemplate",
  "settingInstanceTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
    "settingInstanceTemplateId": "Setting Instance Template Id value",
    "settingDefinitionId": "Setting Definition Id value",
    "isRequired": true,
    "simpleSettingValueTemplate": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
      "settingValueTemplateId": "Setting Value Template Id value",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
        "constantValue": "Constant Value value"
      }
    }
  }
}
```

### <a name="response"></a><span data-ttu-id="64a6b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="64a6b-145">Response</span></span>
<span data-ttu-id="64a6b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64a6b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 833

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingTemplate",
  "id": "203fd028-d028-203f-28d0-3f2028d03f20",
  "settingInstanceTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
    "settingInstanceTemplateId": "Setting Instance Template Id value",
    "settingDefinitionId": "Setting Definition Id value",
    "isRequired": true,
    "simpleSettingValueTemplate": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
      "settingValueTemplateId": "Setting Value Template Id value",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
        "constantValue": "Constant Value value"
      }
    }
  }
}
```




