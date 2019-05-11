---
title: Obter iosDerivedCredentialAuthenticationConfiguration
description: Leia as propriedades e as relações do objeto iosDerivedCredentialAuthenticationConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d82f2d96f2582d4c09ed1e91e63a76a50a6502d9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33956868"
---
# <a name="get-iosderivedcredentialauthenticationconfiguration"></a><span data-ttu-id="ab660-103">Obter iosDerivedCredentialAuthenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab660-103">Get iosDerivedCredentialAuthenticationConfiguration</span></span>

> <span data-ttu-id="ab660-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ab660-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab660-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab660-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab660-106">Leia as propriedades e as relações do objeto [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ab660-106">Read properties and relationships of the [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab660-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ab660-107">Prerequisites</span></span>
<span data-ttu-id="ab660-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab660-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab660-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab660-110">Permission type</span></span>|<span data-ttu-id="ab660-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ab660-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab660-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab660-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab660-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab660-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ab660-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab660-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab660-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab660-115">Not supported.</span></span>|
|<span data-ttu-id="ab660-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab660-116">Application</span></span>|<span data-ttu-id="ab660-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab660-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab660-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab660-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab660-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab660-119">Optional query parameters</span></span>
<span data-ttu-id="ab660-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab660-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab660-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab660-121">Request headers</span></span>
|<span data-ttu-id="ab660-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab660-122">Header</span></span>|<span data-ttu-id="ab660-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ab660-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab660-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab660-124">Authorization</span></span>|<span data-ttu-id="ab660-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab660-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab660-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ab660-126">Accept</span></span>|<span data-ttu-id="ab660-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ab660-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab660-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab660-128">Request body</span></span>
<span data-ttu-id="ab660-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab660-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab660-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab660-130">Response</span></span>
<span data-ttu-id="ab660-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab660-131">If successful, this method returns a `200 OK` response code and [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab660-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab660-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab660-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab660-133">Request</span></span>
<span data-ttu-id="ab660-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab660-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ab660-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab660-135">Response</span></span>
<span data-ttu-id="ab660-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab660-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 490

{
  "value": {
    "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
    "id": "01713f58-3f58-0171-583f-7101583f7101",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```




