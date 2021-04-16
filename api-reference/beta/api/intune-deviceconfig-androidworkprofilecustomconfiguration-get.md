---
title: Obter androidWorkProfileCustomConfiguration
description: Leia propriedades e relações do objeto androidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 14a49df003a3c8a9d80eda32a7f37f063a3bd6b6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864540"
---
# <a name="get-androidworkprofilecustomconfiguration"></a><span data-ttu-id="6a010-103">Obter androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a010-103">Get androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="6a010-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a010-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a010-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a010-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a010-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a010-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a010-107">Leia propriedades e relações do [objeto androidWorkProfileCustomConfiguration.](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a010-107">Read properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a010-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a010-108">Prerequisites</span></span>
<span data-ttu-id="6a010-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a010-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a010-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a010-111">Permission type</span></span>|<span data-ttu-id="6a010-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a010-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a010-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a010-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a010-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a010-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a010-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a010-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a010-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a010-116">Not supported.</span></span>|
|<span data-ttu-id="6a010-117">Application</span><span class="sxs-lookup"><span data-stu-id="6a010-117">Application</span></span>|<span data-ttu-id="6a010-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a010-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a010-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a010-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a010-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a010-120">Optional query parameters</span></span>
<span data-ttu-id="6a010-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a010-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a010-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a010-122">Request headers</span></span>
|<span data-ttu-id="6a010-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a010-123">Header</span></span>|<span data-ttu-id="6a010-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6a010-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a010-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a010-125">Authorization</span></span>|<span data-ttu-id="6a010-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a010-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a010-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a010-127">Accept</span></span>|<span data-ttu-id="6a010-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6a010-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a010-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a010-129">Request body</span></span>
<span data-ttu-id="6a010-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a010-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a010-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a010-131">Response</span></span>
<span data-ttu-id="6a010-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a010-132">If successful, this method returns a `200 OK` response code and [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a010-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a010-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a010-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a010-134">Request</span></span>
<span data-ttu-id="6a010-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a010-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6a010-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a010-136">Response</span></span>
<span data-ttu-id="6a010-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a010-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1623

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
    "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSetting",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "secretReferenceValueId": "Secret Reference Value Id value",
        "isEncrypted": true
      }
    ]
  }
}
```




