---
title: Acessar iosCertificateProfile
description: Leia as propriedades e as relações do objeto iosCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0561870d54b8a26205ff13e87fd8ce99cb00b2e0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967311"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="8e655-103">Acessar iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8e655-103">Get iosCertificateProfile</span></span>

> <span data-ttu-id="8e655-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e655-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e655-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e655-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e655-106">Leia as propriedades e as relações do objeto [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8e655-106">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e655-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e655-107">Prerequisites</span></span>
<span data-ttu-id="8e655-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e655-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e655-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e655-110">Permission type</span></span>|<span data-ttu-id="8e655-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e655-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e655-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e655-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e655-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e655-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8e655-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e655-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e655-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e655-115">Not supported.</span></span>|
|<span data-ttu-id="8e655-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e655-116">Application</span></span>|<span data-ttu-id="8e655-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e655-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e655-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e655-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeSigningCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeEncryptionCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e655-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8e655-119">Optional query parameters</span></span>
<span data-ttu-id="8e655-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8e655-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e655-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e655-121">Request headers</span></span>
|<span data-ttu-id="8e655-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e655-122">Header</span></span>|<span data-ttu-id="8e655-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8e655-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e655-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e655-124">Authorization</span></span>|<span data-ttu-id="8e655-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e655-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e655-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e655-126">Accept</span></span>|<span data-ttu-id="8e655-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8e655-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e655-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e655-128">Request body</span></span>
<span data-ttu-id="8e655-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e655-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e655-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e655-130">Response</span></span>
<span data-ttu-id="8e655-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e655-131">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e655-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e655-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e655-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e655-133">Request</span></span>
<span data-ttu-id="8e655-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e655-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeSigningCertificate
```

### <a name="response"></a><span data-ttu-id="8e655-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e655-135">Response</span></span>
<span data-ttu-id="8e655-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e655-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1279

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
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
    "version": 7
  }
}
```





