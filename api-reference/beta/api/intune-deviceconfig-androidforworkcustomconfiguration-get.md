---
title: Obter androidForWorkCustomConfiguration
description: Leia as propriedades e os relacionamentos do objeto androidForWorkCustomConfiguration.
ms.openlocfilehash: df5272ba06c049b7e69f62098afbd256cda5a78a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038051"
---
# <a name="get-androidforworkcustomconfiguration"></a><span data-ttu-id="c7f11-103">Obter androidForWorkCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7f11-103">Get androidForWorkCustomConfiguration</span></span>

> <span data-ttu-id="c7f11-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c7f11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7f11-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c7f11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7f11-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c7f11-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7f11-107">Leia as propriedades e os relacionamentos do objeto [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c7f11-107">Read properties and relationships of the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7f11-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7f11-108">Prerequisites</span></span>
<span data-ttu-id="c7f11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7f11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7f11-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7f11-111">Permission type</span></span>|<span data-ttu-id="c7f11-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7f11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7f11-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7f11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7f11-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7f11-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c7f11-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7f11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7f11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7f11-116">Not supported.</span></span>|
|<span data-ttu-id="c7f11-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7f11-117">Application</span></span>|<span data-ttu-id="c7f11-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7f11-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7f11-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7f11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7f11-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7f11-120">Optional query parameters</span></span>
<span data-ttu-id="c7f11-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7f11-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c7f11-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7f11-122">Request headers</span></span>
|<span data-ttu-id="c7f11-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7f11-123">Header</span></span>|<span data-ttu-id="c7f11-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c7f11-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7f11-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7f11-125">Authorization</span></span>|<span data-ttu-id="c7f11-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7f11-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7f11-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c7f11-127">Accept</span></span>|<span data-ttu-id="c7f11-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c7f11-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7f11-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7f11-129">Request body</span></span>
<span data-ttu-id="c7f11-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7f11-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7f11-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7f11-131">Response</span></span>
<span data-ttu-id="c7f11-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7f11-132">If successful, this method returns a `200 OK` response code and [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7f11-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7f11-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7f11-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7f11-134">Request</span></span>
<span data-ttu-id="c7f11-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7f11-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c7f11-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7f11-136">Response</span></span>
<span data-ttu-id="c7f11-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7f11-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 732

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
    "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSettingInteger",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "value": 5
      }
    ]
  }
}
```





