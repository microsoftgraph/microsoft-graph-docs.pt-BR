---
title: Listar windows81SCEPCertificateProfiles
description: Listar Propriedades e relações dos objetos windows81SCEPCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ae86d83add4a5dbb50c040f06fbdf8ded728f6ab
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181984"
---
# <a name="list-windows81scepcertificateprofiles"></a><span data-ttu-id="2b111-103">Listar windows81SCEPCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="2b111-103">List windows81SCEPCertificateProfiles</span></span>

> <span data-ttu-id="2b111-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b111-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b111-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b111-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b111-106">Listar Propriedades e relações dos objetos [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2b111-106">List properties and relationships of the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b111-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b111-107">Prerequisites</span></span>
<span data-ttu-id="2b111-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b111-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b111-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b111-110">Permission type</span></span>|<span data-ttu-id="2b111-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b111-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b111-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b111-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b111-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b111-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2b111-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b111-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b111-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b111-115">Not supported.</span></span>|
|<span data-ttu-id="2b111-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b111-116">Application</span></span>|<span data-ttu-id="2b111-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b111-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b111-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b111-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2b111-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b111-119">Request headers</span></span>
|<span data-ttu-id="2b111-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b111-120">Header</span></span>|<span data-ttu-id="2b111-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2b111-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b111-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b111-122">Authorization</span></span>|<span data-ttu-id="2b111-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b111-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b111-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b111-124">Accept</span></span>|<span data-ttu-id="2b111-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2b111-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b111-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b111-126">Request body</span></span>
<span data-ttu-id="2b111-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2b111-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b111-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b111-128">Response</span></span>
<span data-ttu-id="2b111-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b111-129">If successful, this method returns a `200 OK` response code and a collection of [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b111-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b111-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b111-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b111-131">Request</span></span>
<span data-ttu-id="2b111-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b111-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2b111-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b111-133">Response</span></span>
<span data-ttu-id="2b111-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b111-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2473

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
      "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
      "keyStorageProvider": "useTpmKspOtherwiseFail",
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
      "customSubjectAlternativeNames": [
        {
          "@odata.type": "microsoft.graph.customSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ],
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "hashAlgorithm": "sha2",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
      "certificateStore": "machine"
    }
  ]
}
```




