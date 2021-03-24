---
title: Listar windowsPhone81CertificateProfileBases
description: Listar propriedades e relações dos objetos windowsPhone81CertificateProfileBase.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c138f63b82f732225985a9c773d48b695224d13d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132349"
---
# <a name="list-windowsphone81certificateprofilebases"></a><span data-ttu-id="ef874-103">Listar windowsPhone81CertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="ef874-103">List windowsPhone81CertificateProfileBases</span></span>

<span data-ttu-id="ef874-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef874-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef874-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef874-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef874-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef874-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef874-107">Listar propriedades e relações dos objetos [windowsPhone81CertificateProfileBase.](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ef874-107">List properties and relationships of the [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef874-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef874-108">Prerequisites</span></span>
<span data-ttu-id="ef874-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef874-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef874-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef874-111">Permission type</span></span>|<span data-ttu-id="ef874-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef874-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef874-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef874-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef874-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef874-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef874-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef874-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef874-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef874-116">Not supported.</span></span>|
|<span data-ttu-id="ef874-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef874-117">Application</span></span>|<span data-ttu-id="ef874-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef874-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef874-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef874-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ef874-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef874-120">Request headers</span></span>
|<span data-ttu-id="ef874-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef874-121">Header</span></span>|<span data-ttu-id="ef874-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef874-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef874-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef874-123">Authorization</span></span>|<span data-ttu-id="ef874-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef874-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef874-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef874-125">Accept</span></span>|<span data-ttu-id="ef874-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef874-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef874-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef874-127">Request body</span></span>
<span data-ttu-id="ef874-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef874-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef874-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef874-129">Response</span></span>
<span data-ttu-id="ef874-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef874-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef874-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef874-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef874-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef874-132">Request</span></span>
<span data-ttu-id="ef874-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef874-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ef874-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef874-134">Response</span></span>
<span data-ttu-id="ef874-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef874-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1887

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CertificateProfileBase",
      "id": "336e97ac-97ac-336e-ac97-6e33ac976e33",
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
      ]
    }
  ]
}
```




