---
title: Listar androidForWorkCertificateProfileBases
description: Listar Propriedades e relações dos objetos androidForWorkCertificateProfileBase.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e8600b27f5c442a758154a151191850274933681
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37176713"
---
# <a name="list-androidforworkcertificateprofilebases"></a><span data-ttu-id="fa975-103">Listar androidForWorkCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="fa975-103">List androidForWorkCertificateProfileBases</span></span>

> <span data-ttu-id="fa975-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fa975-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa975-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa975-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa975-106">Listar Propriedades e relações dos objetos [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="fa975-106">List properties and relationships of the [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa975-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa975-107">Prerequisites</span></span>
<span data-ttu-id="fa975-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa975-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa975-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa975-110">Permission type</span></span>|<span data-ttu-id="fa975-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fa975-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa975-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa975-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa975-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa975-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fa975-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa975-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa975-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa975-115">Not supported.</span></span>|
|<span data-ttu-id="fa975-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa975-116">Application</span></span>|<span data-ttu-id="fa975-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa975-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa975-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa975-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa975-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa975-119">Request headers</span></span>
|<span data-ttu-id="fa975-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa975-120">Header</span></span>|<span data-ttu-id="fa975-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fa975-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa975-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa975-122">Authorization</span></span>|<span data-ttu-id="fa975-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa975-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa975-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa975-124">Accept</span></span>|<span data-ttu-id="fa975-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa975-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa975-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa975-126">Request body</span></span>
<span data-ttu-id="fa975-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa975-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa975-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa975-128">Response</span></span>
<span data-ttu-id="fa975-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa975-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa975-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa975-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa975-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa975-131">Request</span></span>
<span data-ttu-id="fa975-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa975-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fa975-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa975-133">Response</span></span>
<span data-ttu-id="fa975-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa975-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1832

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkCertificateProfileBase",
      "id": "87f1d53b-d53b-87f1-3bd5-f1873bd5f187",
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
      "subjectAlternativeNameType": "emailAddress"
    }
  ]
}
```




