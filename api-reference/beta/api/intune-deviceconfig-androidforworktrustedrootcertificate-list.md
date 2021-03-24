---
title: Listar androidForWorkTrustedRootCertificates
description: Listar propriedades e relações dos objetos androidForWorkTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 006d3025977b79e28d2b9811e024353e49b54e40
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138257"
---
# <a name="list-androidforworktrustedrootcertificates"></a><span data-ttu-id="479a9-103">Listar androidForWorkTrustedRootCertificates</span><span class="sxs-lookup"><span data-stu-id="479a9-103">List androidForWorkTrustedRootCertificates</span></span>

<span data-ttu-id="479a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="479a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="479a9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="479a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="479a9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="479a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="479a9-107">Listar propriedades e relações dos [objetos androidForWorkTrustedRootCertificate.](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="479a9-107">List properties and relationships of the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="479a9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="479a9-108">Prerequisites</span></span>
<span data-ttu-id="479a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="479a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="479a9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="479a9-111">Permission type</span></span>|<span data-ttu-id="479a9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="479a9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="479a9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="479a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="479a9-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="479a9-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="479a9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="479a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="479a9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="479a9-116">Not supported.</span></span>|
|<span data-ttu-id="479a9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="479a9-117">Application</span></span>|<span data-ttu-id="479a9-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="479a9-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="479a9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="479a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="479a9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="479a9-120">Request headers</span></span>
|<span data-ttu-id="479a9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="479a9-121">Header</span></span>|<span data-ttu-id="479a9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="479a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="479a9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="479a9-123">Authorization</span></span>|<span data-ttu-id="479a9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="479a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="479a9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="479a9-125">Accept</span></span>|<span data-ttu-id="479a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="479a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="479a9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="479a9-127">Request body</span></span>
<span data-ttu-id="479a9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="479a9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="479a9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="479a9-129">Response</span></span>
<span data-ttu-id="479a9-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="479a9-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="479a9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="479a9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="479a9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="479a9-132">Request</span></span>
<span data-ttu-id="479a9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="479a9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="479a9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="479a9-134">Response</span></span>
<span data-ttu-id="479a9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="479a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1488

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
      "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
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
      "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
      "certFileName": "Cert File Name value"
    }
  ]
}
```




