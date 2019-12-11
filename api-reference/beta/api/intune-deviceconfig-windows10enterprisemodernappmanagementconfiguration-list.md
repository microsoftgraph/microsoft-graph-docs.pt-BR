---
title: Listar windows10EnterpriseModernAppManagementConfigurations
description: Listar propriedades e relações dos objetos windows10EnterpriseModernAppManagementConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d04121255f2bebfd0ebb64f0a6f5d43aa5e9328f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947460"
---
# <a name="list-windows10enterprisemodernappmanagementconfigurations"></a><span data-ttu-id="fa11b-103">Listar windows10EnterpriseModernAppManagementConfigurations</span><span class="sxs-lookup"><span data-stu-id="fa11b-103">List windows10EnterpriseModernAppManagementConfigurations</span></span>

> <span data-ttu-id="fa11b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fa11b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa11b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa11b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa11b-106">Listar propriedades e relações dos objetos [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa11b-106">List properties and relationships of the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa11b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa11b-107">Prerequisites</span></span>
<span data-ttu-id="fa11b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa11b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa11b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa11b-110">Permission type</span></span>|<span data-ttu-id="fa11b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fa11b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa11b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa11b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa11b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa11b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fa11b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa11b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa11b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa11b-115">Not supported.</span></span>|
|<span data-ttu-id="fa11b-116">Application</span><span class="sxs-lookup"><span data-stu-id="fa11b-116">Application</span></span>|<span data-ttu-id="fa11b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa11b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa11b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa11b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa11b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa11b-119">Request headers</span></span>
|<span data-ttu-id="fa11b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa11b-120">Header</span></span>|<span data-ttu-id="fa11b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fa11b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa11b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa11b-122">Authorization</span></span>|<span data-ttu-id="fa11b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa11b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa11b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa11b-124">Accept</span></span>|<span data-ttu-id="fa11b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa11b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa11b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa11b-126">Request body</span></span>
<span data-ttu-id="fa11b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa11b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa11b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa11b-128">Response</span></span>
<span data-ttu-id="fa11b-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa11b-129">If successful, this method returns a `200 OK` response code and a collection of [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa11b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa11b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa11b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa11b-131">Request</span></span>
<span data-ttu-id="fa11b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa11b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fa11b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa11b-133">Response</span></span>
<span data-ttu-id="fa11b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa11b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1424

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
      "id": "d6577687-7687-d657-8776-57d6877657d6",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "uninstallBuiltInApps": true
    }
  ]
}
```





