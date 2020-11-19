---
title: Obter macOSExtensionsConfiguration
description: Leia as propriedades e as relações do objeto macOSExtensionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f23ca74536d00ac9f2245de63cb1572851ee7ef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49290933"
---
# <a name="get-macosextensionsconfiguration"></a><span data-ttu-id="65090-103">Obter macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="65090-103">Get macOSExtensionsConfiguration</span></span>

<span data-ttu-id="65090-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65090-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65090-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65090-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65090-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65090-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65090-107">Leia as propriedades e as relações do objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="65090-107">Read properties and relationships of the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65090-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65090-108">Prerequisites</span></span>
<span data-ttu-id="65090-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65090-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65090-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65090-111">Permission type</span></span>|<span data-ttu-id="65090-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65090-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65090-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65090-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65090-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="65090-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="65090-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65090-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65090-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65090-116">Not supported.</span></span>|
|<span data-ttu-id="65090-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65090-117">Application</span></span>|<span data-ttu-id="65090-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="65090-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65090-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65090-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65090-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="65090-120">Optional query parameters</span></span>
<span data-ttu-id="65090-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="65090-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65090-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65090-122">Request headers</span></span>
|<span data-ttu-id="65090-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65090-123">Header</span></span>|<span data-ttu-id="65090-124">Valor</span><span class="sxs-lookup"><span data-stu-id="65090-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65090-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="65090-125">Authorization</span></span>|<span data-ttu-id="65090-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65090-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65090-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="65090-127">Accept</span></span>|<span data-ttu-id="65090-128">application/json</span><span class="sxs-lookup"><span data-stu-id="65090-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65090-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65090-129">Request body</span></span>
<span data-ttu-id="65090-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65090-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65090-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="65090-131">Response</span></span>
<span data-ttu-id="65090-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65090-132">If successful, this method returns a `200 OK` response code and [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65090-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65090-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="65090-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65090-134">Request</span></span>
<span data-ttu-id="65090-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65090-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="65090-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="65090-136">Response</span></span>
<span data-ttu-id="65090-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65090-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2278

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
    "id": "c273f4f6-f4f6-c273-f6f4-73c2f6f473c2",
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
    "kernelExtensionOverridesAllowed": true,
    "kernelExtensionAllowedTeamIdentifiers": [
      "Kernel Extension Allowed Team Identifiers value"
    ],
    "kernelExtensionsAllowed": [
      {
        "@odata.type": "microsoft.graph.macOSKernelExtension",
        "teamIdentifier": "Team Identifier value",
        "bundleId": "Bundle Id value"
      }
    ],
    "systemExtensionsBlockOverride": true,
    "systemExtensionsAllowedTeamIdentifiers": [
      "System Extensions Allowed Team Identifiers value"
    ],
    "systemExtensionsAllowed": [
      {
        "@odata.type": "microsoft.graph.macOSSystemExtension",
        "teamIdentifier": "Team Identifier value",
        "bundleId": "Bundle Id value"
      }
    ],
    "systemExtensionsAllowedTypes": [
      {
        "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
        "teamIdentifier": "Team Identifier value",
        "allowedTypes": "networkExtensionsAllowed"
      }
    ]
  }
}
```




