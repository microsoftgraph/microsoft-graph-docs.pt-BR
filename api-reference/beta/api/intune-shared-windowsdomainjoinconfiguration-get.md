---
title: Obter windowsDomainJoinConfiguration
description: Leia as propriedades e os relacionamentos do objeto windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d0c4aedf07e8a6e95dc81f440975809e75b85160
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831329"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="1fde6-103">Obter windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="1fde6-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="1fde6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1fde6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fde6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1fde6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fde6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1fde6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1fde6-107">Leia as propriedades e os relacionamentos do objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1fde6-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fde6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1fde6-108">Prerequisites</span></span>

<span data-ttu-id="1fde6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fde6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fde6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fde6-111">Permission type</span></span>|<span data-ttu-id="1fde6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1fde6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fde6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fde6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1fde6-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="1fde6-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="1fde6-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fde6-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="1fde6-116">&nbsp; &nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="1fde6-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="1fde6-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fde6-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="1fde6-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fde6-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fde6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fde6-119">Not supported.</span></span>|
|<span data-ttu-id="1fde6-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fde6-120">Application</span></span>|<span data-ttu-id="1fde6-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fde6-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fde6-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fde6-122">HTTP Request</span></span>
<span data-ttu-id="1fde6-123">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="1fde6-123">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="1fde6-124">**Registro**</span><span class="sxs-lookup"><span data-stu-id="1fde6-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1fde6-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1fde6-125">Optional query parameters</span></span>

<span data-ttu-id="1fde6-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1fde6-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fde6-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fde6-127">Request headers</span></span>

|<span data-ttu-id="1fde6-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1fde6-128">Header</span></span>|<span data-ttu-id="1fde6-129">Valor</span><span class="sxs-lookup"><span data-stu-id="1fde6-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fde6-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fde6-130">Authorization</span></span>|<span data-ttu-id="1fde6-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fde6-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fde6-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1fde6-132">Accept</span></span>|<span data-ttu-id="1fde6-133">application/json</span><span class="sxs-lookup"><span data-stu-id="1fde6-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fde6-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fde6-134">Request body</span></span>

<span data-ttu-id="1fde6-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1fde6-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fde6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fde6-136">Response</span></span>

<span data-ttu-id="1fde6-137">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fde6-137">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fde6-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fde6-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fde6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fde6-139">Request</span></span>

<span data-ttu-id="1fde6-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fde6-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1fde6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fde6-141">Response</span></span>

<span data-ttu-id="1fde6-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fde6-142">Here is an example of the response.</span></span> <span data-ttu-id="1fde6-143">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="1fde6-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1fde6-144">Propriedades retornadas de uma chamada real dependem do contexto.</span><span class="sxs-lookup"><span data-stu-id="1fde6-144">Properties returned from an actual call depend on the context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
    "id": "40118d08-8d08-4011-088d-1140088d1140",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "computerNameStaticPrefix": "Computer Name Static Prefix value",
    "computerNameSuffixRandomCharCount": 1,
    "activeDirectoryDomainName": "Active Directory Domain Name value"
  }
}
```



