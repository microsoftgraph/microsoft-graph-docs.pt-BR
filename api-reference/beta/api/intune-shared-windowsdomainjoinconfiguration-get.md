---
title: Obter windowsDomainJoinConfiguration
description: Leia as propriedades e as relações do objeto windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ac435dd5edf3854d994fb2fc3aa7bd0c7f8bc7a
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085455"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="79054-103">Obter windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="79054-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="79054-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="79054-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="79054-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="79054-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79054-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79054-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79054-107">Leia as propriedades e as relações do objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="79054-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79054-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79054-108">Prerequisites</span></span>

<span data-ttu-id="79054-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79054-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79054-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79054-111">Permission type</span></span>|<span data-ttu-id="79054-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79054-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79054-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79054-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="79054-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="79054-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="79054-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79054-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="79054-116">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="79054-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="79054-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="79054-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="79054-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79054-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79054-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79054-119">Not supported.</span></span>|
|<span data-ttu-id="79054-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79054-120">Application</span></span>||
| <span data-ttu-id="79054-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="79054-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="79054-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79054-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="79054-123">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="79054-123">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="79054-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="79054-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79054-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79054-125">HTTP Request</span></span>
<span data-ttu-id="79054-126">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="79054-126">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="79054-127">**Enrollmentid**</span><span class="sxs-lookup"><span data-stu-id="79054-127">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79054-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79054-128">Optional query parameters</span></span>

<span data-ttu-id="79054-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="79054-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79054-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79054-130">Request headers</span></span>

|<span data-ttu-id="79054-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79054-131">Header</span></span>|<span data-ttu-id="79054-132">Valor</span><span class="sxs-lookup"><span data-stu-id="79054-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79054-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="79054-133">Authorization</span></span>|<span data-ttu-id="79054-134">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79054-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79054-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79054-135">Accept</span></span>|<span data-ttu-id="79054-136">application/json</span><span class="sxs-lookup"><span data-stu-id="79054-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79054-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79054-137">Request body</span></span>

<span data-ttu-id="79054-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="79054-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79054-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="79054-139">Response</span></span>

<span data-ttu-id="79054-140">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79054-140">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79054-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79054-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="79054-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79054-142">Request</span></span>

<span data-ttu-id="79054-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79054-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="79054-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="79054-144">Response</span></span>

<span data-ttu-id="79054-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79054-145">Here is an example of the response.</span></span> <span data-ttu-id="79054-146">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="79054-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="79054-147">As propriedades retornadas de uma chamada real dependem do contexto.</span><span class="sxs-lookup"><span data-stu-id="79054-147">Properties returned from an actual call depend on the context.</span></span>

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












