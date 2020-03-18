---
title: Listar androidForWorkPkcsCertificateProfiles
description: Listar Propriedades e relações dos objetos androidForWorkPkcsCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: abb34c6f0d0cc2412a6129569073c563591d3643
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759173"
---
# <a name="list-androidforworkpkcscertificateprofiles"></a><span data-ttu-id="21812-103">Listar androidForWorkPkcsCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="21812-103">List androidForWorkPkcsCertificateProfiles</span></span>

> <span data-ttu-id="21812-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21812-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21812-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21812-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21812-106">Listar Propriedades e relações dos objetos [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="21812-106">List properties and relationships of the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21812-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21812-107">Prerequisites</span></span>
<span data-ttu-id="21812-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21812-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21812-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21812-110">Permission type</span></span>|<span data-ttu-id="21812-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21812-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21812-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21812-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21812-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21812-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="21812-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21812-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21812-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21812-115">Not supported.</span></span>|
|<span data-ttu-id="21812-116">Application</span><span class="sxs-lookup"><span data-stu-id="21812-116">Application</span></span>|<span data-ttu-id="21812-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21812-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21812-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21812-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="21812-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21812-119">Request headers</span></span>
|<span data-ttu-id="21812-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21812-120">Header</span></span>|<span data-ttu-id="21812-121">Valor</span><span class="sxs-lookup"><span data-stu-id="21812-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21812-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="21812-122">Authorization</span></span>|<span data-ttu-id="21812-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21812-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21812-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21812-124">Accept</span></span>|<span data-ttu-id="21812-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21812-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21812-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21812-126">Request body</span></span>
<span data-ttu-id="21812-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21812-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21812-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="21812-128">Response</span></span>
<span data-ttu-id="21812-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21812-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21812-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21812-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="21812-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21812-131">Request</span></span>
<span data-ttu-id="21812-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21812-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="21812-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="21812-133">Response</span></span>
<span data-ttu-id="21812-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21812-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2135

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
      "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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
      "certificationAuthority": "Certification Authority value",
      "certificationAuthorityName": "Certification Authority Name value",
      "certificateTemplateName": "Certificate Template Name value",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
    }
  ]
}
```




