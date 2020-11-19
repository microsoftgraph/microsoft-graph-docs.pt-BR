---
title: Listar androidDeviceOwnerCertificateProfileBases
description: Listar Propriedades e relações dos objetos androidDeviceOwnerCertificateProfileBase.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b8356f26983cc454180ddba36e105501662964a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242928"
---
# <a name="list-androiddeviceownercertificateprofilebases"></a><span data-ttu-id="09f33-103">Listar androidDeviceOwnerCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="09f33-103">List androidDeviceOwnerCertificateProfileBases</span></span>

<span data-ttu-id="09f33-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09f33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09f33-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09f33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09f33-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09f33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09f33-107">Listar Propriedades e relações dos objetos [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="09f33-107">List properties and relationships of the [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09f33-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09f33-108">Prerequisites</span></span>
<span data-ttu-id="09f33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09f33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09f33-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09f33-111">Permission type</span></span>|<span data-ttu-id="09f33-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09f33-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09f33-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09f33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09f33-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="09f33-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="09f33-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09f33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09f33-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09f33-116">Not supported.</span></span>|
|<span data-ttu-id="09f33-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09f33-117">Application</span></span>|<span data-ttu-id="09f33-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="09f33-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09f33-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09f33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="09f33-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09f33-120">Request headers</span></span>
|<span data-ttu-id="09f33-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09f33-121">Header</span></span>|<span data-ttu-id="09f33-122">Valor</span><span class="sxs-lookup"><span data-stu-id="09f33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09f33-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="09f33-123">Authorization</span></span>|<span data-ttu-id="09f33-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09f33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09f33-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09f33-125">Accept</span></span>|<span data-ttu-id="09f33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09f33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09f33-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09f33-127">Request body</span></span>
<span data-ttu-id="09f33-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09f33-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09f33-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="09f33-129">Response</span></span>
<span data-ttu-id="09f33-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09f33-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09f33-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09f33-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="09f33-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09f33-132">Request</span></span>
<span data-ttu-id="09f33-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09f33-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="09f33-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="09f33-134">Response</span></span>
<span data-ttu-id="09f33-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09f33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1836

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerCertificateProfileBase",
      "id": "19dd17f0-17f0-19dd-f017-dd19f017dd19",
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
      "renewalThresholdPercentage": 10,
      "subjectNameFormat": "commonNameIncludingEmail",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "subjectAlternativeNameType": "emailAddress"
    }
  ]
}
```




