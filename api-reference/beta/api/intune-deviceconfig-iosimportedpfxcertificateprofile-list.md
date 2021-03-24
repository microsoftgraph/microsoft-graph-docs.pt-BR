---
title: Listar iosImportedPFXCertificateProfiles
description: Listar propriedades e relações dos objetos iosImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 44b2747312ce030d5fbdceeea24809c13035ab00
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147837"
---
# <a name="list-iosimportedpfxcertificateprofiles"></a><span data-ttu-id="ae049-103">Listar iosImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="ae049-103">List iosImportedPFXCertificateProfiles</span></span>

<span data-ttu-id="ae049-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae049-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae049-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae049-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae049-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae049-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae049-107">Listar propriedades e relações dos [objetos iosImportedPFXCertificateProfile.](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ae049-107">List properties and relationships of the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae049-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae049-108">Prerequisites</span></span>
<span data-ttu-id="ae049-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae049-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae049-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae049-111">Permission type</span></span>|<span data-ttu-id="ae049-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae049-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae049-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae049-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae049-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae049-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae049-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae049-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae049-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae049-116">Not supported.</span></span>|
|<span data-ttu-id="ae049-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae049-117">Application</span></span>|<span data-ttu-id="ae049-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae049-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae049-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae049-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ae049-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae049-120">Request headers</span></span>
|<span data-ttu-id="ae049-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae049-121">Header</span></span>|<span data-ttu-id="ae049-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ae049-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae049-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae049-123">Authorization</span></span>|<span data-ttu-id="ae049-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae049-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae049-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae049-125">Accept</span></span>|<span data-ttu-id="ae049-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae049-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae049-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae049-127">Request body</span></span>
<span data-ttu-id="ae049-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae049-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae049-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae049-129">Response</span></span>
<span data-ttu-id="ae049-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae049-130">If successful, this method returns a `200 OK` response code and a collection of [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae049-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae049-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae049-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae049-132">Request</span></span>
<span data-ttu-id="ae049-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae049-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ae049-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae049-134">Response</span></span>
<span data-ttu-id="ae049-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae049-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1413

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
      "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
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
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```




