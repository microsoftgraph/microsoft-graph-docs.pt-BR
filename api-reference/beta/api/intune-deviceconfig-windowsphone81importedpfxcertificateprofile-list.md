---
title: Listar windowsPhone81ImportedPFXCertificateProfiles
description: Listar propriedades e relações dos objetos windowsPhone81ImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5db6cbc47b669f19e807c05148b10f829e1e96b1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154774"
---
# <a name="list-windowsphone81importedpfxcertificateprofiles"></a><span data-ttu-id="f4aad-103">Listar windowsPhone81ImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="f4aad-103">List windowsPhone81ImportedPFXCertificateProfiles</span></span>

<span data-ttu-id="f4aad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4aad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4aad-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4aad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4aad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4aad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4aad-107">Listar propriedades e relações dos objetos [windowsPhone81ImportedPFXCertificateProfile.](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4aad-107">List properties and relationships of the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4aad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4aad-108">Prerequisites</span></span>
<span data-ttu-id="f4aad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4aad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4aad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4aad-111">Permission type</span></span>|<span data-ttu-id="f4aad-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4aad-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4aad-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4aad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4aad-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4aad-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4aad-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4aad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4aad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4aad-116">Not supported.</span></span>|
|<span data-ttu-id="f4aad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4aad-117">Application</span></span>|<span data-ttu-id="f4aad-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4aad-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4aad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4aad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f4aad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4aad-120">Request headers</span></span>
|<span data-ttu-id="f4aad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4aad-121">Header</span></span>|<span data-ttu-id="f4aad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f4aad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4aad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4aad-123">Authorization</span></span>|<span data-ttu-id="f4aad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4aad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4aad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4aad-125">Accept</span></span>|<span data-ttu-id="f4aad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4aad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4aad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4aad-127">Request body</span></span>
<span data-ttu-id="f4aad-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f4aad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4aad-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4aad-129">Response</span></span>
<span data-ttu-id="f4aad-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4aad-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4aad-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4aad-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4aad-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4aad-132">Request</span></span>
<span data-ttu-id="f4aad-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4aad-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f4aad-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4aad-134">Response</span></span>
<span data-ttu-id="f4aad-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4aad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1725

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
      "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
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
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```




