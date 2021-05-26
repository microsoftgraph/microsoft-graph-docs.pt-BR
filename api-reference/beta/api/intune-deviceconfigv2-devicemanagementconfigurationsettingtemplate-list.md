---
title: Listar deviceManagementConfigurationSettingTemplates
description: Listar propriedades e relações dos objetos deviceManagementConfigurationSettingTemplate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99591f65be18681cdd02cd9b8f4f77557cd374a5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664819"
---
# <a name="list-devicemanagementconfigurationsettingtemplates"></a><span data-ttu-id="e05db-103">Listar deviceManagementConfigurationSettingTemplates</span><span class="sxs-lookup"><span data-stu-id="e05db-103">List deviceManagementConfigurationSettingTemplates</span></span>

<span data-ttu-id="e05db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e05db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e05db-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e05db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e05db-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e05db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e05db-107">Listar propriedades e relações dos [objetos deviceManagementConfigurationSettingTemplate.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e05db-107">List properties and relationships of the [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e05db-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e05db-108">Prerequisites</span></span>
<span data-ttu-id="e05db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e05db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e05db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e05db-111">Permission type</span></span>|<span data-ttu-id="e05db-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e05db-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e05db-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e05db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e05db-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e05db-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e05db-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e05db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e05db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e05db-116">Not supported.</span></span>|
|<span data-ttu-id="e05db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e05db-117">Application</span></span>|<span data-ttu-id="e05db-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e05db-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e05db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e05db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templateSettings
GET /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates
```

## <a name="request-headers"></a><span data-ttu-id="e05db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e05db-120">Request headers</span></span>
|<span data-ttu-id="e05db-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e05db-121">Header</span></span>|<span data-ttu-id="e05db-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e05db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e05db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e05db-123">Authorization</span></span>|<span data-ttu-id="e05db-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e05db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e05db-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e05db-125">Accept</span></span>|<span data-ttu-id="e05db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e05db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e05db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e05db-127">Request body</span></span>
<span data-ttu-id="e05db-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e05db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e05db-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e05db-129">Response</span></span>
<span data-ttu-id="e05db-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e05db-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e05db-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e05db-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e05db-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e05db-132">Request</span></span>
<span data-ttu-id="e05db-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e05db-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templateSettings
```

### <a name="response"></a><span data-ttu-id="e05db-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e05db-134">Response</span></span>
<span data-ttu-id="e05db-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e05db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 930

{
  "value": [
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
  ]
}
```




