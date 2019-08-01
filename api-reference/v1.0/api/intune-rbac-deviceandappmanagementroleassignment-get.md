---
title: Obter deviceAndAppManagementRoleAssignment
description: Ler propriedades de leitura e relações do objeto deviceAndAppManagementRoleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b5f22b134d1bc7d1f6e83e7a5f2b96f3974ad9b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023906"
---
# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="d8225-103">Obter deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d8225-103">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="d8225-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8225-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8225-105">Ler propriedades de leitura e relações do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d8225-105">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8225-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8225-106">Prerequisites</span></span>
<span data-ttu-id="d8225-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8225-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8225-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8225-109">Permission type</span></span>|<span data-ttu-id="d8225-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8225-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8225-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8225-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8225-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8225-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="d8225-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8225-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8225-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8225-114">Not supported.</span></span>|
|<span data-ttu-id="d8225-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8225-115">Application</span></span>|<span data-ttu-id="d8225-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8225-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8225-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8225-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8225-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d8225-118">Optional query parameters</span></span>
<span data-ttu-id="d8225-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d8225-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8225-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8225-120">Request headers</span></span>
|<span data-ttu-id="d8225-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8225-121">Header</span></span>|<span data-ttu-id="d8225-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d8225-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8225-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8225-123">Authorization</span></span>|<span data-ttu-id="d8225-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8225-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8225-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8225-125">Accept</span></span>|<span data-ttu-id="d8225-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8225-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8225-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8225-127">Request body</span></span>
<span data-ttu-id="d8225-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8225-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8225-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8225-129">Response</span></span>
<span data-ttu-id="d8225-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8225-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8225-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8225-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8225-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8225-132">Request</span></span>
<span data-ttu-id="d8225-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8225-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d8225-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8225-134">Response</span></span>
<span data-ttu-id="d8225-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8225-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
    "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
    "displayName": "Display Name value",
    "description": "Description value",
    "resourceScopes": [
      "Resource Scopes value"
    ],
    "members": [
      "Members value"
    ]
  }
}
```



