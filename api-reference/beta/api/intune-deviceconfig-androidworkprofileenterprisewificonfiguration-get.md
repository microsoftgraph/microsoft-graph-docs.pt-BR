---
title: Obter androidWorkProfileEnterpriseWiFiConfiguration
description: Leia as propriedades e as relações do objeto androidWorkProfileEnterpriseWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 064ccab43e12be908b7ac2876eb56a577faa411d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32475218"
---
# <a name="get-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="a1208-103">Obter androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1208-103">Get androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="a1208-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1208-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1208-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1208-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1208-106">Leia as propriedades e as relações do objeto [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a1208-106">Read properties and relationships of the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1208-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1208-107">Prerequisites</span></span>
<span data-ttu-id="a1208-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1208-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1208-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1208-110">Permission type</span></span>|<span data-ttu-id="a1208-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1208-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1208-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1208-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1208-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1208-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a1208-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1208-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1208-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1208-115">Not supported.</span></span>|
|<span data-ttu-id="a1208-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1208-116">Application</span></span>|<span data-ttu-id="a1208-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1208-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1208-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1208-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1208-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1208-119">Optional query parameters</span></span>
<span data-ttu-id="a1208-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1208-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1208-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1208-121">Request headers</span></span>
|<span data-ttu-id="a1208-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1208-122">Header</span></span>|<span data-ttu-id="a1208-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a1208-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1208-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1208-124">Authorization</span></span>|<span data-ttu-id="a1208-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1208-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1208-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1208-126">Accept</span></span>|<span data-ttu-id="a1208-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a1208-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1208-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1208-128">Request body</span></span>
<span data-ttu-id="a1208-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1208-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1208-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1208-130">Response</span></span>
<span data-ttu-id="a1208-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1208-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1208-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1208-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1208-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1208-133">Request</span></span>
<span data-ttu-id="a1208-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1208-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a1208-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1208-135">Response</span></span>
<span data-ttu-id="a1208-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1208-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1009

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
    "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "networkName": "Network Name value",
    "ssid": "Ssid value",
    "connectAutomatically": true,
    "connectWhenNetworkNameIsHidden": true,
    "wiFiSecurityType": "wpaEnterprise",
    "eapType": "eapTtls",
    "authenticationMethod": "usernameAndPassword",
    "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
    "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
    "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
  }
}
```





