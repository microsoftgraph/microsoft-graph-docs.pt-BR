---
title: Obter androidImportedPFXCertificateProfile
description: Leia as propriedades e as relações do objeto androidImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64456c28852e4c208e7d8ad777f7557c48247438
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43344518"
---
# <a name="get-androidimportedpfxcertificateprofile"></a><span data-ttu-id="fd75f-103">Obter androidImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="fd75f-103">Get androidImportedPFXCertificateProfile</span></span>

<span data-ttu-id="fd75f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd75f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd75f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fd75f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd75f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd75f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd75f-107">Leia as propriedades e as relações do objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fd75f-107">Read properties and relationships of the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd75f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd75f-108">Prerequisites</span></span>
<span data-ttu-id="fd75f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd75f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd75f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd75f-111">Permission type</span></span>|<span data-ttu-id="fd75f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd75f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd75f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd75f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd75f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd75f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fd75f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd75f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd75f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd75f-116">Not supported.</span></span>|
|<span data-ttu-id="fd75f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd75f-117">Application</span></span>|<span data-ttu-id="fd75f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd75f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd75f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd75f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd75f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fd75f-120">Optional query parameters</span></span>
<span data-ttu-id="fd75f-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fd75f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd75f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd75f-122">Request headers</span></span>
|<span data-ttu-id="fd75f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd75f-123">Header</span></span>|<span data-ttu-id="fd75f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fd75f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd75f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd75f-125">Authorization</span></span>|<span data-ttu-id="fd75f-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd75f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd75f-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd75f-127">Accept</span></span>|<span data-ttu-id="fd75f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fd75f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd75f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd75f-129">Request body</span></span>
<span data-ttu-id="fd75f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fd75f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd75f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd75f-131">Response</span></span>
<span data-ttu-id="fd75f-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd75f-132">If successful, this method returns a `200 OK` response code and [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd75f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd75f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd75f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd75f-134">Request</span></span>
<span data-ttu-id="fd75f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd75f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="fd75f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd75f-136">Response</span></span>
<span data-ttu-id="fd75f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd75f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1773

{
  "value": {
    "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
    "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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
}
```



