---
title: Acessar windows10CustomConfiguration
description: Leia as propriedades e as relações do objeto windows10CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d45a31b3fe03eaa1c3e9cf31f2b8f99e7fc4675d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866486"
---
# <a name="get-windows10customconfiguration"></a><span data-ttu-id="01f08-103">Acessar windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="01f08-103">Get windows10CustomConfiguration</span></span>

<span data-ttu-id="01f08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01f08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01f08-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01f08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01f08-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01f08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01f08-107">Leia as propriedades e as relações do objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01f08-107">Read properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01f08-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01f08-108">Prerequisites</span></span>
<span data-ttu-id="01f08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01f08-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01f08-111">Permission type</span></span>|<span data-ttu-id="01f08-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01f08-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01f08-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01f08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01f08-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f08-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01f08-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01f08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01f08-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01f08-116">Not supported.</span></span>|
|<span data-ttu-id="01f08-117">Application</span><span class="sxs-lookup"><span data-stu-id="01f08-117">Application</span></span>|<span data-ttu-id="01f08-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f08-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01f08-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01f08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01f08-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="01f08-120">Optional query parameters</span></span>
<span data-ttu-id="01f08-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="01f08-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01f08-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01f08-122">Request headers</span></span>
|<span data-ttu-id="01f08-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01f08-123">Header</span></span>|<span data-ttu-id="01f08-124">Valor</span><span class="sxs-lookup"><span data-stu-id="01f08-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01f08-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="01f08-125">Authorization</span></span>|<span data-ttu-id="01f08-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01f08-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01f08-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01f08-127">Accept</span></span>|<span data-ttu-id="01f08-128">application/json</span><span class="sxs-lookup"><span data-stu-id="01f08-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01f08-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01f08-129">Request body</span></span>
<span data-ttu-id="01f08-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01f08-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01f08-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="01f08-131">Response</span></span>
<span data-ttu-id="01f08-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01f08-132">If successful, this method returns a `200 OK` response code and [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01f08-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01f08-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="01f08-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01f08-134">Request</span></span>
<span data-ttu-id="01f08-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01f08-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="01f08-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="01f08-136">Response</span></span>
<span data-ttu-id="01f08-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01f08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1614

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
    "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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




