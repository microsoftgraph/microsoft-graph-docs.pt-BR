---
title: Lista iosEnterpriseWiFiConfigurations
description: Lista as propriedades e os relacionamentos dos objetos iosEnterpriseWiFiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b085c9d0b798221035dd7bcc74eae16feb9acb6f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419538"
---
# <a name="list-iosenterprisewificonfigurations"></a><span data-ttu-id="f94c4-103">Lista iosEnterpriseWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="f94c4-103">List iosEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="f94c4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f94c4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f94c4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f94c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f94c4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f94c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f94c4-107">Lista as propriedades e os relacionamentos dos objetos [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f94c4-107">List properties and relationships of the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f94c4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f94c4-108">Prerequisites</span></span>
<span data-ttu-id="f94c4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f94c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f94c4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f94c4-111">Permission type</span></span>|<span data-ttu-id="f94c4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f94c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f94c4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f94c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f94c4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f94c4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f94c4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f94c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f94c4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f94c4-116">Not supported.</span></span>|
|<span data-ttu-id="f94c4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f94c4-117">Application</span></span>|<span data-ttu-id="f94c4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f94c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f94c4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f94c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f94c4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f94c4-120">Request headers</span></span>
|<span data-ttu-id="f94c4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f94c4-121">Header</span></span>|<span data-ttu-id="f94c4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f94c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f94c4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f94c4-123">Authorization</span></span>|<span data-ttu-id="f94c4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f94c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f94c4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f94c4-125">Accept</span></span>|<span data-ttu-id="f94c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f94c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f94c4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f94c4-127">Request body</span></span>
<span data-ttu-id="f94c4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f94c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f94c4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f94c4-129">Response</span></span>
<span data-ttu-id="f94c4-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f94c4-130">If successful, this method returns a `200 OK` response code and a collection of [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f94c4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f94c4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f94c4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f94c4-132">Request</span></span>
<span data-ttu-id="f94c4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f94c4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f94c4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f94c4-134">Response</span></span>
<span data-ttu-id="f94c4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f94c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




