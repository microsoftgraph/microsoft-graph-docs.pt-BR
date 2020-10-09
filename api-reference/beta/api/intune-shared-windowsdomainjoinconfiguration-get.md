---
title: Obter windowsDomainJoinConfiguration
description: Leia as propriedades e as relações do objeto windowsDomainJoinConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e25511c308bce1a27e5579e8c61adbc7e7c8e8af
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404004"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="bdf69-103">Obter windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdf69-103">Get windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="bdf69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdf69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdf69-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bdf69-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bdf69-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bdf69-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdf69-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bdf69-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdf69-108">Leia as propriedades e as relações do objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bdf69-108">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdf69-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bdf69-109">Prerequisites</span></span>

<span data-ttu-id="bdf69-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdf69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdf69-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdf69-112">Permission type</span></span>|<span data-ttu-id="bdf69-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bdf69-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdf69-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdf69-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bdf69-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="bdf69-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="bdf69-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdf69-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="bdf69-117">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="bdf69-117">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="bdf69-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdf69-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="bdf69-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdf69-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdf69-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdf69-120">Not supported.</span></span>|
|<span data-ttu-id="bdf69-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdf69-121">Application</span></span>||
| <span data-ttu-id="bdf69-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="bdf69-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="bdf69-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdf69-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="bdf69-124">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="bdf69-124">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="bdf69-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdf69-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdf69-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdf69-126">HTTP Request</span></span>
<span data-ttu-id="bdf69-127">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="bdf69-127">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="bdf69-128">**Enrollmentid**</span><span class="sxs-lookup"><span data-stu-id="bdf69-128">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bdf69-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bdf69-129">Optional query parameters</span></span>

<span data-ttu-id="bdf69-130">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf69-130">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bdf69-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf69-131">Request headers</span></span>

|<span data-ttu-id="bdf69-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bdf69-132">Header</span></span>|<span data-ttu-id="bdf69-133">Valor</span><span class="sxs-lookup"><span data-stu-id="bdf69-133">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdf69-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdf69-134">Authorization</span></span>|<span data-ttu-id="bdf69-135">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdf69-135">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdf69-136">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bdf69-136">Accept</span></span>|<span data-ttu-id="bdf69-137">application/json</span><span class="sxs-lookup"><span data-stu-id="bdf69-137">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdf69-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf69-138">Request body</span></span>

<span data-ttu-id="bdf69-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bdf69-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdf69-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf69-140">Response</span></span>

<span data-ttu-id="bdf69-141">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf69-141">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdf69-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdf69-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdf69-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf69-143">Request</span></span>

<span data-ttu-id="bdf69-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdf69-144">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bdf69-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf69-145">Response</span></span>

<span data-ttu-id="bdf69-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf69-146">Here is an example of the response.</span></span> <span data-ttu-id="bdf69-147">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="bdf69-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bdf69-148">As propriedades retornadas de uma chamada real dependem do contexto.</span><span class="sxs-lookup"><span data-stu-id="bdf69-148">Properties returned from an actual call depend on the context.</span></span>

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