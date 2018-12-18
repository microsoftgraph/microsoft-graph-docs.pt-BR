---
title: Acessar iosCustomConfiguration
description: Leia as propriedades e as relações do objeto iosCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: aab8af4cbdaff832327f7d92474b88f453b47e10
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355111"
---
# <a name="get-ioscustomconfiguration"></a><span data-ttu-id="e8916-103">Acessar iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="e8916-103">Get iosCustomConfiguration</span></span>

> <span data-ttu-id="e8916-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8916-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8916-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8916-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8916-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e8916-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8916-107">Leia as propriedades e as relações do objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e8916-107">Read properties and relationships of the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8916-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8916-108">Prerequisites</span></span>
<span data-ttu-id="e8916-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8916-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8916-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8916-111">Permission type</span></span>|<span data-ttu-id="e8916-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8916-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8916-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8916-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8916-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8916-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e8916-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8916-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8916-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8916-116">Not supported.</span></span>|
|<span data-ttu-id="e8916-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8916-117">Application</span></span>|<span data-ttu-id="e8916-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8916-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8916-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8916-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8916-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8916-120">Optional query parameters</span></span>
<span data-ttu-id="e8916-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8916-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e8916-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8916-122">Request headers</span></span>
|<span data-ttu-id="e8916-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8916-123">Header</span></span>|<span data-ttu-id="e8916-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e8916-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8916-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8916-125">Authorization</span></span>|<span data-ttu-id="e8916-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8916-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8916-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e8916-127">Accept</span></span>|<span data-ttu-id="e8916-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e8916-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8916-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8916-129">Request body</span></span>
<span data-ttu-id="e8916-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8916-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8916-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8916-131">Response</span></span>
<span data-ttu-id="e8916-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8916-132">If successful, this method returns a `200 OK` response code and [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8916-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8916-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8916-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8916-134">Request</span></span>
<span data-ttu-id="e8916-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8916-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e8916-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8916-136">Response</span></span>
<span data-ttu-id="e8916-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8916-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCustomConfiguration",
    "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "payloadName": "Payload Name value",
    "payloadFileName": "Payload File Name value",
    "payload": "cGF5bG9hZA=="
  }
}
```





