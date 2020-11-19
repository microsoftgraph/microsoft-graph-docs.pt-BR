---
title: Listar windowsPhone81SCEPCertificateProfiles
description: Listar Propriedades e relações dos objetos windowsPhone81SCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 502d82ec0b9f44e31a9c0b77423c1d56ffefad54
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49290515"
---
# <a name="list-windowsphone81scepcertificateprofiles"></a><span data-ttu-id="73648-103">Listar windowsPhone81SCEPCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="73648-103">List windowsPhone81SCEPCertificateProfiles</span></span>

<span data-ttu-id="73648-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73648-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73648-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73648-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73648-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73648-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73648-107">Listar Propriedades e relações dos objetos [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="73648-107">List properties and relationships of the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73648-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73648-108">Prerequisites</span></span>
<span data-ttu-id="73648-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73648-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73648-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73648-111">Permission type</span></span>|<span data-ttu-id="73648-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73648-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73648-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73648-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73648-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73648-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73648-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73648-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73648-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73648-116">Not supported.</span></span>|
|<span data-ttu-id="73648-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73648-117">Application</span></span>|<span data-ttu-id="73648-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73648-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73648-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73648-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="73648-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73648-120">Request headers</span></span>
|<span data-ttu-id="73648-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73648-121">Header</span></span>|<span data-ttu-id="73648-122">Valor</span><span class="sxs-lookup"><span data-stu-id="73648-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73648-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="73648-123">Authorization</span></span>|<span data-ttu-id="73648-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73648-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73648-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73648-125">Accept</span></span>|<span data-ttu-id="73648-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73648-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73648-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73648-127">Request body</span></span>
<span data-ttu-id="73648-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73648-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73648-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="73648-129">Response</span></span>
<span data-ttu-id="73648-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73648-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73648-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73648-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="73648-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73648-132">Request</span></span>
<span data-ttu-id="73648-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73648-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="73648-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="73648-134">Response</span></span>
<span data-ttu-id="73648-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73648-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2222

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
      "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "hashAlgorithm": "sha2",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
    }
  ]
}
```




