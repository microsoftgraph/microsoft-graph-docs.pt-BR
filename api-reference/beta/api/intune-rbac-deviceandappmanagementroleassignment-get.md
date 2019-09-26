---
title: Obter deviceAndAppManagementRoleAssignment
description: Ler propriedades de leitura e relações do objeto deviceAndAppManagementRoleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 41d0b698f56be152293cfa967c2d37a78ad25e48
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189638"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="e8b20-103">Obter deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e8b20-103">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="e8b20-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8b20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8b20-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8b20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8b20-106">Ler propriedades de leitura e relações do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e8b20-106">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8b20-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8b20-107">Prerequisites</span></span>
<span data-ttu-id="e8b20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8b20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8b20-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8b20-110">Permission type</span></span>|<span data-ttu-id="e8b20-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8b20-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8b20-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8b20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8b20-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8b20-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e8b20-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8b20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8b20-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8b20-115">Not supported.</span></span>|
|<span data-ttu-id="e8b20-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8b20-116">Application</span></span>|<span data-ttu-id="e8b20-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8b20-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8b20-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8b20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8b20-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8b20-119">Optional query parameters</span></span>
<span data-ttu-id="e8b20-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8b20-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8b20-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b20-121">Request headers</span></span>
|<span data-ttu-id="e8b20-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8b20-122">Header</span></span>|<span data-ttu-id="e8b20-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e8b20-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8b20-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8b20-124">Authorization</span></span>|<span data-ttu-id="e8b20-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8b20-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8b20-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8b20-126">Accept</span></span>|<span data-ttu-id="e8b20-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e8b20-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8b20-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b20-128">Request body</span></span>
<span data-ttu-id="e8b20-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8b20-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8b20-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8b20-130">Response</span></span>
<span data-ttu-id="e8b20-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8b20-131">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8b20-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8b20-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8b20-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8b20-133">Request</span></span>
<span data-ttu-id="e8b20-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8b20-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e8b20-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8b20-135">Response</span></span>
<span data-ttu-id="e8b20-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8b20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
    "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
    "displayName": "Display Name value",
    "description": "Description value",
    "scopeMembers": [
      "Scope Members value"
    ],
    "scopeType": "allDevices",
    "resourceScopes": [
      "Resource Scopes value"
    ],
    "members": [
      "Members value"
    ]
  }
}
```




