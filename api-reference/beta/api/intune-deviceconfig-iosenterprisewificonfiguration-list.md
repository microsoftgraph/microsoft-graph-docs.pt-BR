---
title: Listar iosEnterpriseWiFiConfigurations
description: Listar Propriedades e relações dos objetos iosEnterpriseWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73edddaef559941041777e651d17e5a0979ab752
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988991"
---
# <a name="list-iosenterprisewificonfigurations"></a><span data-ttu-id="8d415-103">Listar iosEnterpriseWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="8d415-103">List iosEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="8d415-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8d415-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d415-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d415-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d415-106">Listar Propriedades e relações dos objetos [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8d415-106">List properties and relationships of the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d415-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d415-107">Prerequisites</span></span>
<span data-ttu-id="8d415-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d415-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d415-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d415-110">Permission type</span></span>|<span data-ttu-id="8d415-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8d415-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d415-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d415-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d415-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d415-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8d415-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d415-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d415-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d415-115">Not supported.</span></span>|
|<span data-ttu-id="8d415-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d415-116">Application</span></span>|<span data-ttu-id="8d415-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d415-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d415-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d415-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8d415-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d415-119">Request headers</span></span>
|<span data-ttu-id="8d415-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d415-120">Header</span></span>|<span data-ttu-id="8d415-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8d415-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d415-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d415-122">Authorization</span></span>|<span data-ttu-id="8d415-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d415-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d415-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d415-124">Accept</span></span>|<span data-ttu-id="8d415-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d415-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d415-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d415-126">Request body</span></span>
<span data-ttu-id="8d415-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d415-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d415-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d415-128">Response</span></span>
<span data-ttu-id="8d415-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d415-129">If successful, this method returns a `200 OK` response code and a collection of [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d415-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d415-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d415-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d415-131">Request</span></span>
<span data-ttu-id="8d415-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d415-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8d415-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d415-133">Response</span></span>
<span data-ttu-id="8d415-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d415-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1404

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
      "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
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
      "wiFiSecurityType": "wpaPersonal",
      "proxySettings": "manual",
      "proxyManualAddress": "Proxy Manual Address value",
      "proxyManualPort": 15,
      "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
      "preSharedKey": "Pre Shared Key value",
      "eapType": "leap",
      "eapFastConfiguration": "useProtectedAccessCredential",
      "trustedServerCertificateNames": [
        "Trusted Server Certificate Names value"
      ],
      "authenticationMethod": "usernameAndPassword",
      "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
    }
  ]
}
```




