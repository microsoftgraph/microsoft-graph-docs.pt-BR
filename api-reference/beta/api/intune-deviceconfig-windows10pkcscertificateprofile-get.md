---
title: Obter windows10PkcsCertificateProfile
description: Leia propriedades e relações do objeto windows10PkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: de676c5ecec56e4c60a177b76d10d9bc7a257d07
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127519"
---
# <a name="get-windows10pkcscertificateprofile"></a><span data-ttu-id="92cfe-103">Obter windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="92cfe-103">Get windows10PkcsCertificateProfile</span></span>

<span data-ttu-id="92cfe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92cfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92cfe-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92cfe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92cfe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92cfe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92cfe-107">Leia propriedades e relações do [objeto windows10PkcsCertificateProfile.](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="92cfe-107">Read properties and relationships of the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92cfe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92cfe-108">Prerequisites</span></span>
<span data-ttu-id="92cfe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92cfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92cfe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92cfe-111">Permission type</span></span>|<span data-ttu-id="92cfe-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92cfe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92cfe-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92cfe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92cfe-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92cfe-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92cfe-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92cfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92cfe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92cfe-116">Not supported.</span></span>|
|<span data-ttu-id="92cfe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92cfe-117">Application</span></span>|<span data-ttu-id="92cfe-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92cfe-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92cfe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92cfe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92cfe-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92cfe-120">Optional query parameters</span></span>
<span data-ttu-id="92cfe-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92cfe-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92cfe-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92cfe-122">Request headers</span></span>
|<span data-ttu-id="92cfe-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92cfe-123">Header</span></span>|<span data-ttu-id="92cfe-124">Valor</span><span class="sxs-lookup"><span data-stu-id="92cfe-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92cfe-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="92cfe-125">Authorization</span></span>|<span data-ttu-id="92cfe-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92cfe-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92cfe-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92cfe-127">Accept</span></span>|<span data-ttu-id="92cfe-128">application/json</span><span class="sxs-lookup"><span data-stu-id="92cfe-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92cfe-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92cfe-129">Request body</span></span>
<span data-ttu-id="92cfe-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92cfe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92cfe-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="92cfe-131">Response</span></span>
<span data-ttu-id="92cfe-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92cfe-132">If successful, this method returns a `200 OK` response code and [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92cfe-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92cfe-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="92cfe-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92cfe-134">Request</span></span>
<span data-ttu-id="92cfe-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92cfe-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="92cfe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="92cfe-136">Response</span></span>
<span data-ttu-id="92cfe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92cfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2381

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
    "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
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
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "subjectNameFormatString": "Subject Name Format String value",
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




