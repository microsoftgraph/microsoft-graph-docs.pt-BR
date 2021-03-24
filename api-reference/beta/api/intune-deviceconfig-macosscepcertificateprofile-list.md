---
title: Listar macOSScepCertificateProfiles
description: Listar propriedades e relações dos objetos macOSScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc2f90ab458301bf9bb0ed21144b57e00aa0d87d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127911"
---
# <a name="list-macosscepcertificateprofiles"></a><span data-ttu-id="ca737-103">Listar macOSScepCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="ca737-103">List macOSScepCertificateProfiles</span></span>

<span data-ttu-id="ca737-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca737-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca737-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca737-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca737-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca737-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca737-107">Listar propriedades e relações dos [objetos macOSScepCertificateProfile.](../resources/intune-deviceconfig-macosscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ca737-107">List properties and relationships of the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca737-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca737-108">Prerequisites</span></span>
<span data-ttu-id="ca737-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca737-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca737-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca737-111">Permission type</span></span>|<span data-ttu-id="ca737-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca737-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca737-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca737-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca737-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca737-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca737-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca737-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca737-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca737-116">Not supported.</span></span>|
|<span data-ttu-id="ca737-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca737-117">Application</span></span>|<span data-ttu-id="ca737-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca737-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca737-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca737-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ca737-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca737-120">Request headers</span></span>
|<span data-ttu-id="ca737-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca737-121">Header</span></span>|<span data-ttu-id="ca737-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ca737-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca737-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca737-123">Authorization</span></span>|<span data-ttu-id="ca737-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca737-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca737-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca737-125">Accept</span></span>|<span data-ttu-id="ca737-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca737-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca737-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca737-127">Request body</span></span>
<span data-ttu-id="ca737-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca737-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca737-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca737-129">Response</span></span>
<span data-ttu-id="ca737-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca737-130">If successful, this method returns a `200 OK` response code and a collection of [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca737-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca737-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca737-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca737-132">Request</span></span>
<span data-ttu-id="ca737-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca737-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ca737-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca737-134">Response</span></span>
<span data-ttu-id="ca737-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca737-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
      "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
      "subjectNameFormat": "commonNameAsEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "hashAlgorithm": "sha2",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
      "certificateStore": "machine",
      "customSubjectAlternativeNames": [
        {
          "@odata.type": "microsoft.graph.customSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ]
    }
  ]
}
```




