---
title: Obter windowsPhone81TrustedRootCertificate
description: Leia as propriedades e as relações do objeto windowsPhone81TrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 536fb9243e2b5b3205b674b061082b7b229a8ad3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42474540"
---
# <a name="get-windowsphone81trustedrootcertificate"></a><span data-ttu-id="befcd-103">Obter windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="befcd-103">Get windowsPhone81TrustedRootCertificate</span></span>

<span data-ttu-id="befcd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="befcd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="befcd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="befcd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="befcd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="befcd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="befcd-107">Leia as propriedades e as relações do objeto [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="befcd-107">Read properties and relationships of the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="befcd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="befcd-108">Prerequisites</span></span>
<span data-ttu-id="befcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="befcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="befcd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="befcd-111">Permission type</span></span>|<span data-ttu-id="befcd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="befcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="befcd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="befcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="befcd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="befcd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="befcd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="befcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="befcd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="befcd-116">Not supported.</span></span>|
|<span data-ttu-id="befcd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="befcd-117">Application</span></span>|<span data-ttu-id="befcd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="befcd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="befcd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="befcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="befcd-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="befcd-120">Optional query parameters</span></span>
<span data-ttu-id="befcd-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="befcd-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="befcd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="befcd-122">Request headers</span></span>
|<span data-ttu-id="befcd-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="befcd-123">Header</span></span>|<span data-ttu-id="befcd-124">Valor</span><span class="sxs-lookup"><span data-stu-id="befcd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="befcd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="befcd-125">Authorization</span></span>|<span data-ttu-id="befcd-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="befcd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="befcd-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="befcd-127">Accept</span></span>|<span data-ttu-id="befcd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="befcd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="befcd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="befcd-129">Request body</span></span>
<span data-ttu-id="befcd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="befcd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="befcd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="befcd-131">Response</span></span>
<span data-ttu-id="befcd-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="befcd-132">If successful, this method returns a `200 OK` response code and [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="befcd-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="befcd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="befcd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="befcd-134">Request</span></span>
<span data-ttu-id="befcd-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="befcd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

### <a name="response"></a><span data-ttu-id="befcd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="befcd-136">Response</span></span>
<span data-ttu-id="befcd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="befcd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1406

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
    "id": "6316bf01-bf01-6316-01bf-166301bf1663",
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
}
```





