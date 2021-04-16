---
title: Listar androidWorkProfileCustomConfigurations
description: Listar propriedades e relações dos objetos androidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b42f899931bb6c1a540e438486070e09c9449d73
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864477"
---
# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="ba5dd-103">Listar androidWorkProfileCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="ba5dd-103">List androidWorkProfileCustomConfigurations</span></span>

<span data-ttu-id="ba5dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba5dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba5dd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba5dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba5dd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba5dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba5dd-107">Listar propriedades e relações dos objetos [androidWorkProfileCustomConfiguration.](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba5dd-107">List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba5dd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba5dd-108">Prerequisites</span></span>
<span data-ttu-id="ba5dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba5dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba5dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba5dd-111">Permission type</span></span>|<span data-ttu-id="ba5dd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba5dd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba5dd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba5dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba5dd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba5dd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba5dd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba5dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba5dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba5dd-116">Not supported.</span></span>|
|<span data-ttu-id="ba5dd-117">Application</span><span class="sxs-lookup"><span data-stu-id="ba5dd-117">Application</span></span>|<span data-ttu-id="ba5dd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba5dd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba5dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba5dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ba5dd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba5dd-120">Request headers</span></span>
|<span data-ttu-id="ba5dd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba5dd-121">Header</span></span>|<span data-ttu-id="ba5dd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ba5dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba5dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba5dd-123">Authorization</span></span>|<span data-ttu-id="ba5dd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba5dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba5dd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba5dd-125">Accept</span></span>|<span data-ttu-id="ba5dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba5dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba5dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba5dd-127">Request body</span></span>
<span data-ttu-id="ba5dd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba5dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba5dd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba5dd-129">Response</span></span>
<span data-ttu-id="ba5dd-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba5dd-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba5dd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba5dd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba5dd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba5dd-132">Request</span></span>
<span data-ttu-id="ba5dd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba5dd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ba5dd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba5dd-134">Response</span></span>
<span data-ttu-id="ba5dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba5dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1721

{
  "value": [
    {
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
  ]
}
```




