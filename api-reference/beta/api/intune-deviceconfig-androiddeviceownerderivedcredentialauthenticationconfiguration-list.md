---
title: Listar androidDeviceOwnerDerivedCredentialAuthenticationConfigurations
description: Listar Propriedades e relações dos objetos androidDeviceOwnerDerivedCredentialAuthenticationConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f42de2c5faf52cb8b6e14968c7edeabb3ba1de26
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242676"
---
# <a name="list-androiddeviceownerderivedcredentialauthenticationconfigurations"></a><span data-ttu-id="6b3ef-103">Listar androidDeviceOwnerDerivedCredentialAuthenticationConfigurations</span><span class="sxs-lookup"><span data-stu-id="6b3ef-103">List androidDeviceOwnerDerivedCredentialAuthenticationConfigurations</span></span>

<span data-ttu-id="6b3ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b3ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b3ef-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b3ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b3ef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b3ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b3ef-107">Listar Propriedades e relações dos objetos [androidDeviceOwnerDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-androiddeviceownerderivedcredentialauthenticationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6b3ef-107">List properties and relationships of the [androidDeviceOwnerDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-androiddeviceownerderivedcredentialauthenticationconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b3ef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b3ef-108">Prerequisites</span></span>
<span data-ttu-id="6b3ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b3ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b3ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b3ef-111">Permission type</span></span>|<span data-ttu-id="6b3ef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b3ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b3ef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b3ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b3ef-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b3ef-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6b3ef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b3ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b3ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b3ef-116">Not supported.</span></span>|
|<span data-ttu-id="6b3ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3ef-117">Application</span></span>|<span data-ttu-id="6b3ef-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b3ef-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b3ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b3ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6b3ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b3ef-120">Request headers</span></span>
|<span data-ttu-id="6b3ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b3ef-121">Header</span></span>|<span data-ttu-id="6b3ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6b3ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b3ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b3ef-123">Authorization</span></span>|<span data-ttu-id="6b3ef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b3ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b3ef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b3ef-125">Accept</span></span>|<span data-ttu-id="6b3ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b3ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b3ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b3ef-127">Request body</span></span>
<span data-ttu-id="6b3ef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b3ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b3ef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b3ef-129">Response</span></span>
<span data-ttu-id="6b3ef-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidDeviceOwnerDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-androiddeviceownerderivedcredentialauthenticationconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b3ef-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-androiddeviceownerderivedcredentialauthenticationconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b3ef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b3ef-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b3ef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b3ef-132">Request</span></span>
<span data-ttu-id="6b3ef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b3ef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6b3ef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b3ef-134">Response</span></span>
<span data-ttu-id="6b3ef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b3ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1398

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerDerivedCredentialAuthenticationConfiguration",
      "id": "9815f155-f155-9815-55f1-159855f11598",
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
      "version": 7
    }
  ]
}
```




