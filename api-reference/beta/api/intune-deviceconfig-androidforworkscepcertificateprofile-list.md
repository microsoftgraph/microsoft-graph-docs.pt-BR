---
title: Listar androidForWorkScepCertificateProfiles
description: Listar Propriedades e relações dos objetos androidForWorkScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2590aa047a8734eb9e54062ca46801c0b569f069
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045352"
---
# <a name="list-androidforworkscepcertificateprofiles"></a><span data-ttu-id="daedd-103">Listar androidForWorkScepCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="daedd-103">List androidForWorkScepCertificateProfiles</span></span>

<span data-ttu-id="daedd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daedd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="daedd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="daedd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daedd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="daedd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daedd-107">Listar Propriedades e relações dos objetos [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="daedd-107">List properties and relationships of the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="daedd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="daedd-108">Prerequisites</span></span>
<span data-ttu-id="daedd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daedd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daedd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="daedd-111">Permission type</span></span>|<span data-ttu-id="daedd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="daedd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daedd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="daedd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="daedd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="daedd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="daedd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="daedd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daedd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daedd-116">Not supported.</span></span>|
|<span data-ttu-id="daedd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="daedd-117">Application</span></span>|<span data-ttu-id="daedd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="daedd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="daedd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="daedd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="daedd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="daedd-120">Request headers</span></span>
|<span data-ttu-id="daedd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="daedd-121">Header</span></span>|<span data-ttu-id="daedd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="daedd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daedd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="daedd-123">Authorization</span></span>|<span data-ttu-id="daedd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="daedd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daedd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="daedd-125">Accept</span></span>|<span data-ttu-id="daedd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="daedd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daedd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="daedd-127">Request body</span></span>
<span data-ttu-id="daedd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="daedd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daedd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="daedd-129">Response</span></span>
<span data-ttu-id="daedd-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="daedd-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daedd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="daedd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="daedd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="daedd-132">Request</span></span>
<span data-ttu-id="daedd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="daedd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="daedd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="daedd-134">Response</span></span>
<span data-ttu-id="daedd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="daedd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2423

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
      "id": "09e532af-32af-09e5-af32-e509af32e509",
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
      "subjectAlternativeNameType": "emailAddress",
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "hashAlgorithm": "sha2",
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






