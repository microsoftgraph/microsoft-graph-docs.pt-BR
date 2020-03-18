---
title: Obter androidForWorkScepCertificateProfile
description: Leia as propriedades e as relações do objeto androidForWorkScepCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0dd35d9fc9cc7d542aa5f7d93806ea27b951707
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759145"
---
# <a name="get-androidforworkscepcertificateprofile"></a><span data-ttu-id="e1743-103">Obter androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="e1743-103">Get androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="e1743-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1743-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1743-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1743-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1743-106">Leia as propriedades e as relações do objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e1743-106">Read properties and relationships of the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1743-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1743-107">Prerequisites</span></span>
<span data-ttu-id="e1743-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1743-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1743-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1743-110">Permission type</span></span>|<span data-ttu-id="e1743-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1743-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1743-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1743-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1743-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1743-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e1743-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1743-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1743-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1743-115">Not supported.</span></span>|
|<span data-ttu-id="e1743-116">Application</span><span class="sxs-lookup"><span data-stu-id="e1743-116">Application</span></span>|<span data-ttu-id="e1743-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1743-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1743-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1743-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1743-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1743-119">Optional query parameters</span></span>
<span data-ttu-id="e1743-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1743-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1743-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1743-121">Request headers</span></span>
|<span data-ttu-id="e1743-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1743-122">Header</span></span>|<span data-ttu-id="e1743-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e1743-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1743-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1743-124">Authorization</span></span>|<span data-ttu-id="e1743-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1743-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1743-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1743-126">Accept</span></span>|<span data-ttu-id="e1743-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e1743-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1743-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1743-128">Request body</span></span>
<span data-ttu-id="e1743-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1743-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1743-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1743-130">Response</span></span>
<span data-ttu-id="e1743-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1743-131">If successful, this method returns a `200 OK` response code and [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1743-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1743-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1743-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1743-133">Request</span></span>
<span data-ttu-id="e1743-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1743-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e1743-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1743-135">Response</span></span>
<span data-ttu-id="e1743-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1743-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2289

{
  "value": {
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
}
```




