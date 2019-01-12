---
title: Lista macOSEnterpriseWiFiConfigurations
description: Lista as propriedades e os relacionamentos dos objetos macOSEnterpriseWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: facd20603e1daa8d907a5f94c1771c480f7f30a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961208"
---
# <a name="list-macosenterprisewificonfigurations"></a><span data-ttu-id="f5675-103">Lista macOSEnterpriseWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="f5675-103">List macOSEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="f5675-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5675-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5675-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5675-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5675-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f5675-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5675-107">Lista as propriedades e os relacionamentos dos objetos [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f5675-107">List properties and relationships of the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5675-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5675-108">Prerequisites</span></span>
<span data-ttu-id="f5675-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5675-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5675-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5675-111">Permission type</span></span>|<span data-ttu-id="f5675-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5675-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5675-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5675-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5675-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5675-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f5675-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5675-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5675-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5675-116">Not supported.</span></span>|
|<span data-ttu-id="f5675-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5675-117">Application</span></span>|<span data-ttu-id="f5675-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5675-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5675-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5675-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f5675-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5675-120">Request headers</span></span>
|<span data-ttu-id="f5675-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5675-121">Header</span></span>|<span data-ttu-id="f5675-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f5675-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5675-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5675-123">Authorization</span></span>|<span data-ttu-id="f5675-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5675-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5675-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5675-125">Accept</span></span>|<span data-ttu-id="f5675-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5675-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5675-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5675-127">Request body</span></span>
<span data-ttu-id="f5675-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5675-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5675-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5675-129">Response</span></span>
<span data-ttu-id="f5675-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5675-130">If successful, this method returns a `200 OK` response code and a collection of [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5675-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5675-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5675-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5675-132">Request</span></span>
<span data-ttu-id="f5675-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5675-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f5675-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5675-134">Response</span></span>
<span data-ttu-id="f5675-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5675-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1406

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
      "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
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





