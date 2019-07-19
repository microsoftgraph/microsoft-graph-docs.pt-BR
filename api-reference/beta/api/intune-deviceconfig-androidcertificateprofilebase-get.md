---
title: Obter androidCertificateProfileBase
description: Leia as propriedades e as relações do objeto androidCertificateProfileBase.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c410c1a08cb40fadf0c5cc95e511a56f1a38940
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971707"
---
# <a name="get-androidcertificateprofilebase"></a><span data-ttu-id="73dbc-103">Obter androidCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="73dbc-103">Get androidCertificateProfileBase</span></span>

> <span data-ttu-id="73dbc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73dbc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73dbc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73dbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73dbc-106">Leia as propriedades e as relações do objeto [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="73dbc-106">Read properties and relationships of the [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73dbc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73dbc-107">Prerequisites</span></span>
<span data-ttu-id="73dbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73dbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73dbc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73dbc-110">Permission type</span></span>|<span data-ttu-id="73dbc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73dbc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73dbc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73dbc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73dbc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73dbc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73dbc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73dbc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73dbc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73dbc-115">Not supported.</span></span>|
|<span data-ttu-id="73dbc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73dbc-116">Application</span></span>|<span data-ttu-id="73dbc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73dbc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73dbc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73dbc-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="73dbc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="73dbc-119">Optional query parameters</span></span>
<span data-ttu-id="73dbc-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="73dbc-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73dbc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73dbc-121">Request headers</span></span>
|<span data-ttu-id="73dbc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73dbc-122">Header</span></span>|<span data-ttu-id="73dbc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="73dbc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73dbc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="73dbc-124">Authorization</span></span>|<span data-ttu-id="73dbc-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73dbc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73dbc-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73dbc-126">Accept</span></span>|<span data-ttu-id="73dbc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="73dbc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73dbc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73dbc-128">Request body</span></span>
<span data-ttu-id="73dbc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73dbc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73dbc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="73dbc-130">Response</span></span>
<span data-ttu-id="73dbc-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73dbc-131">If successful, this method returns a `200 OK` response code and [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73dbc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73dbc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="73dbc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73dbc-133">Request</span></span>
<span data-ttu-id="73dbc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73dbc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidVpnConfiguration/identityCertificate
```

### <a name="response"></a><span data-ttu-id="73dbc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="73dbc-135">Response</span></span>
<span data-ttu-id="73dbc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73dbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





