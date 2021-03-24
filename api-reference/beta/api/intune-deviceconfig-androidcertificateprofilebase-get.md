---
title: Obter androidCertificateProfileBase
description: Leia propriedades e relações do objeto androidCertificateProfileBase.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 50611a53ef3469ba3fbc1a01109a32728b829293
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126819"
---
# <a name="get-androidcertificateprofilebase"></a><span data-ttu-id="c6677-103">Obter androidCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="c6677-103">Get androidCertificateProfileBase</span></span>

<span data-ttu-id="c6677-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6677-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6677-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6677-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6677-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6677-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6677-107">Leia propriedades e relações do [objeto androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c6677-107">Read properties and relationships of the [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6677-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6677-108">Prerequisites</span></span>
<span data-ttu-id="c6677-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6677-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6677-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6677-111">Permission type</span></span>|<span data-ttu-id="c6677-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6677-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6677-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6677-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6677-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6677-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c6677-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6677-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6677-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6677-116">Not supported.</span></span>|
|<span data-ttu-id="c6677-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6677-117">Application</span></span>|<span data-ttu-id="c6677-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6677-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6677-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6677-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidVpnConfiguration/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEasEmailProfileConfiguration/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEasEmailProfileConfiguration/smimeSigningCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c6677-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c6677-120">Optional query parameters</span></span>
<span data-ttu-id="c6677-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c6677-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6677-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6677-122">Request headers</span></span>
|<span data-ttu-id="c6677-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6677-123">Header</span></span>|<span data-ttu-id="c6677-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c6677-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6677-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6677-125">Authorization</span></span>|<span data-ttu-id="c6677-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6677-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6677-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c6677-127">Accept</span></span>|<span data-ttu-id="c6677-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c6677-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6677-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6677-129">Request body</span></span>
<span data-ttu-id="c6677-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6677-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6677-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6677-131">Response</span></span>
<span data-ttu-id="c6677-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6677-132">If successful, this method returns a `200 OK` response code and [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6677-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6677-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6677-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6677-134">Request</span></span>
<span data-ttu-id="c6677-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6677-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidVpnConfiguration/identityCertificate
```

### <a name="response"></a><span data-ttu-id="c6677-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6677-136">Response</span></span>
<span data-ttu-id="c6677-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6677-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1723

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCertificateProfileBase",
    "id": "76cf241d-241d-76cf-1d24-cf761d24cf76",
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
    ]
  }
}
```




