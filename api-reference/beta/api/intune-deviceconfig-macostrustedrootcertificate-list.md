---
title: Listar macOSTrustedRootCertificates
description: Listar Propriedades e relações dos objetos macOSTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb3e9e8304e3bdd0b193c34a5da037ce41e97b4b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792748"
---
# <a name="list-macostrustedrootcertificates"></a><span data-ttu-id="92bb6-103">Listar macOSTrustedRootCertificates</span><span class="sxs-lookup"><span data-stu-id="92bb6-103">List macOSTrustedRootCertificates</span></span>

<span data-ttu-id="92bb6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92bb6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92bb6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92bb6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92bb6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92bb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92bb6-107">Listar Propriedades e relações dos objetos [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="92bb6-107">List properties and relationships of the [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92bb6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92bb6-108">Prerequisites</span></span>
<span data-ttu-id="92bb6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92bb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92bb6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92bb6-111">Permission type</span></span>|<span data-ttu-id="92bb6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92bb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92bb6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92bb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92bb6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92bb6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="92bb6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92bb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92bb6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92bb6-116">Not supported.</span></span>|
|<span data-ttu-id="92bb6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92bb6-117">Application</span></span>|<span data-ttu-id="92bb6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92bb6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92bb6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92bb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="92bb6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92bb6-120">Request headers</span></span>
|<span data-ttu-id="92bb6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92bb6-121">Header</span></span>|<span data-ttu-id="92bb6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92bb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92bb6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92bb6-123">Authorization</span></span>|<span data-ttu-id="92bb6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92bb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92bb6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92bb6-125">Accept</span></span>|<span data-ttu-id="92bb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92bb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92bb6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92bb6-127">Request body</span></span>
<span data-ttu-id="92bb6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92bb6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92bb6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="92bb6-129">Response</span></span>
<span data-ttu-id="92bb6-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92bb6-130">If successful, this method returns a `200 OK` response code and a collection of [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92bb6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92bb6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="92bb6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92bb6-132">Request</span></span>
<span data-ttu-id="92bb6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92bb6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSEnterpriseWiFiConfiguration/rootCertificatesForServerValidation
```

### <a name="response"></a><span data-ttu-id="92bb6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="92bb6-134">Response</span></span>
<span data-ttu-id="92bb6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92bb6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1479

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
      "id": "c5fac954-c954-c5fa-54c9-fac554c9fac5",
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
      "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
      "certFileName": "Cert File Name value"
    }
  ]
}
```



