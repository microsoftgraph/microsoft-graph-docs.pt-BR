---
title: Obter windowsDomainJoinConfiguration
description: Leia propriedades e relações do objeto windowsDomainJoinConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7e331d74999eff64663b5e7bd86959e718a6eca4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866942"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="16b0e-103">Obter windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="16b0e-103">Get windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="16b0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16b0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16b0e-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="16b0e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16b0e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16b0e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16b0e-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16b0e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16b0e-108">Leia propriedades e relações do [objeto windowsDomainJoinConfiguration.](../resources/intune-shared-windowsdomainjoinconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16b0e-108">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16b0e-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16b0e-109">Prerequisites</span></span>

<span data-ttu-id="16b0e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16b0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16b0e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16b0e-112">Permission type</span></span>|<span data-ttu-id="16b0e-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16b0e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16b0e-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16b0e-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="16b0e-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="16b0e-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="16b0e-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16b0e-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="16b0e-117">&nbsp;&nbsp; **Inscrição**</span><span class="sxs-lookup"><span data-stu-id="16b0e-117">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="16b0e-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="16b0e-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="16b0e-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16b0e-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16b0e-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16b0e-120">Not supported.</span></span>|
|<span data-ttu-id="16b0e-121">Application</span><span class="sxs-lookup"><span data-stu-id="16b0e-121">Application</span></span>||
| <span data-ttu-id="16b0e-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="16b0e-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="16b0e-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="16b0e-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="16b0e-124">&nbsp;&nbsp; **Inscrição**</span><span class="sxs-lookup"><span data-stu-id="16b0e-124">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="16b0e-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="16b0e-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16b0e-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16b0e-126">HTTP Request</span></span>
<span data-ttu-id="16b0e-127">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="16b0e-127">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="16b0e-128">**Inscrição**</span><span class="sxs-lookup"><span data-stu-id="16b0e-128">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16b0e-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="16b0e-129">Optional query parameters</span></span>

<span data-ttu-id="16b0e-130">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="16b0e-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16b0e-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16b0e-131">Request headers</span></span>

|<span data-ttu-id="16b0e-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16b0e-132">Header</span></span>|<span data-ttu-id="16b0e-133">Valor</span><span class="sxs-lookup"><span data-stu-id="16b0e-133">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16b0e-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="16b0e-134">Authorization</span></span>|<span data-ttu-id="16b0e-135">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16b0e-135">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16b0e-136">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16b0e-136">Accept</span></span>|<span data-ttu-id="16b0e-137">application/json</span><span class="sxs-lookup"><span data-stu-id="16b0e-137">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16b0e-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16b0e-138">Request body</span></span>

<span data-ttu-id="16b0e-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16b0e-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16b0e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="16b0e-140">Response</span></span>

<span data-ttu-id="16b0e-141">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16b0e-141">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16b0e-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16b0e-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="16b0e-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16b0e-143">Request</span></span>

<span data-ttu-id="16b0e-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16b0e-144">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="16b0e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="16b0e-145">Response</span></span>

<span data-ttu-id="16b0e-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16b0e-146">Here is an example of the response.</span></span> <span data-ttu-id="16b0e-147">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="16b0e-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16b0e-148">As propriedades retornadas de uma chamada real dependem do contexto.</span><span class="sxs-lookup"><span data-stu-id="16b0e-148">Properties returned from an actual call depend on the context.</span></span>

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










