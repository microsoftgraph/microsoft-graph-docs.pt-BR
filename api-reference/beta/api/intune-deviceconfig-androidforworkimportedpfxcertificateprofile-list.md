---
title: Listar androidForWorkImportedPFXCertificateProfiles
description: Listar propriedades e relações dos objetos androidForWorkImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b66b4e5d821dc71aa4959381085f8283a6413293
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142608"
---
# <a name="list-androidforworkimportedpfxcertificateprofiles"></a><span data-ttu-id="fdeb1-103">Listar androidForWorkImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="fdeb1-103">List androidForWorkImportedPFXCertificateProfiles</span></span>

<span data-ttu-id="fdeb1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdeb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdeb1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fdeb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdeb1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fdeb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdeb1-107">Listar propriedades e relações dos [objetos androidForWorkImportedPFXCertificateProfile.](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdeb1-107">List properties and relationships of the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdeb1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fdeb1-108">Prerequisites</span></span>
<span data-ttu-id="fdeb1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdeb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdeb1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdeb1-111">Permission type</span></span>|<span data-ttu-id="fdeb1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdeb1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdeb1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdeb1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdeb1-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdeb1-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fdeb1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdeb1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdeb1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdeb1-116">Not supported.</span></span>|
|<span data-ttu-id="fdeb1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdeb1-117">Application</span></span>|<span data-ttu-id="fdeb1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdeb1-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdeb1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdeb1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fdeb1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdeb1-120">Request headers</span></span>
|<span data-ttu-id="fdeb1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdeb1-121">Header</span></span>|<span data-ttu-id="fdeb1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fdeb1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdeb1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdeb1-123">Authorization</span></span>|<span data-ttu-id="fdeb1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdeb1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdeb1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdeb1-125">Accept</span></span>|<span data-ttu-id="fdeb1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdeb1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdeb1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdeb1-127">Request body</span></span>
<span data-ttu-id="fdeb1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdeb1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdeb1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdeb1-129">Response</span></span>
<span data-ttu-id="fdeb1-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdeb1-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdeb1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdeb1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdeb1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdeb1-132">Request</span></span>
<span data-ttu-id="fdeb1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdeb1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fdeb1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdeb1-134">Response</span></span>
<span data-ttu-id="fdeb1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdeb1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1884

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
      "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
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
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```




