---
title: Obter deviceAndAppManagementRoleAssignment
description: Ler propriedades de leitura e relações do objeto deviceAndAppManagementRoleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0fa225c571ef3572d3002019cd0d0e3d026c6ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460042"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="eeab2-103">Obter deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="eeab2-103">Get deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="eeab2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eeab2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eeab2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eeab2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eeab2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eeab2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeab2-107">Ler propriedades de leitura e relações do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eeab2-107">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eeab2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eeab2-108">Prerequisites</span></span>
<span data-ttu-id="eeab2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeab2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeab2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eeab2-111">Permission type</span></span>|<span data-ttu-id="eeab2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eeab2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eeab2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eeab2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eeab2-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="eeab2-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="eeab2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eeab2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eeab2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eeab2-116">Not supported.</span></span>|
|<span data-ttu-id="eeab2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eeab2-117">Application</span></span>|<span data-ttu-id="eeab2-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="eeab2-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eeab2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eeab2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eeab2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eeab2-120">Optional query parameters</span></span>
<span data-ttu-id="eeab2-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eeab2-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eeab2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eeab2-122">Request headers</span></span>
|<span data-ttu-id="eeab2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eeab2-123">Header</span></span>|<span data-ttu-id="eeab2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="eeab2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eeab2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="eeab2-125">Authorization</span></span>|<span data-ttu-id="eeab2-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eeab2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eeab2-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eeab2-127">Accept</span></span>|<span data-ttu-id="eeab2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="eeab2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeab2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eeab2-129">Request body</span></span>
<span data-ttu-id="eeab2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eeab2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eeab2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="eeab2-131">Response</span></span>
<span data-ttu-id="eeab2-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eeab2-132">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeab2-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eeab2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="eeab2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eeab2-134">Request</span></span>
<span data-ttu-id="eeab2-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eeab2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="eeab2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="eeab2-136">Response</span></span>
<span data-ttu-id="eeab2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eeab2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





