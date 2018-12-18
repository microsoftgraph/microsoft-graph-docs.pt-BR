---
title: Obter macOSEndpointProtectionConfiguration
description: Leia as propriedades e os relacionamentos do objeto macOSEndpointProtectionConfiguration.
author: tfitzmac
ms.openlocfilehash: 90d96b8acc210d0fa04f34b72606de5913554243
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325155"
---
# <a name="get-macosendpointprotectionconfiguration"></a><span data-ttu-id="5e746-103">Obter macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e746-103">Get macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="5e746-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5e746-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e746-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5e746-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e746-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5e746-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e746-107">Leia as propriedades e os relacionamentos do objeto [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5e746-107">Read properties and relationships of the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e746-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e746-108">Prerequisites</span></span>
<span data-ttu-id="5e746-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e746-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e746-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e746-111">Permission type</span></span>|<span data-ttu-id="5e746-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5e746-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e746-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e746-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e746-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e746-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5e746-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e746-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e746-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e746-116">Not supported.</span></span>|
|<span data-ttu-id="5e746-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e746-117">Application</span></span>|<span data-ttu-id="5e746-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e746-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e746-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e746-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e746-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5e746-120">Optional query parameters</span></span>
<span data-ttu-id="5e746-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5e746-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5e746-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e746-122">Request headers</span></span>
|<span data-ttu-id="5e746-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e746-123">Header</span></span>|<span data-ttu-id="5e746-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5e746-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e746-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e746-125">Authorization</span></span>|<span data-ttu-id="5e746-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e746-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e746-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5e746-127">Accept</span></span>|<span data-ttu-id="5e746-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5e746-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e746-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e746-129">Request body</span></span>
<span data-ttu-id="5e746-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e746-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e746-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e746-131">Response</span></span>
<span data-ttu-id="5e746-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e746-132">If successful, this method returns a `200 OK` response code and [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e746-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e746-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e746-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e746-134">Request</span></span>
<span data-ttu-id="5e746-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e746-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5e746-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e746-136">Response</span></span>
<span data-ttu-id="5e746-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e746-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 884

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
    "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "gatekeeperAllowedAppSource": "macAppStore",
    "gatekeeperBlockOverride": true,
    "firewallEnabled": true,
    "firewallBlockAllIncoming": true,
    "firewallEnableStealthMode": true,
    "firewallApplications": [
      {
        "@odata.type": "microsoft.graph.macOSFirewallApplication",
        "bundleId": "Bundle Id value",
        "allowsIncomingConnections": true
      }
    ]
  }
}
```





