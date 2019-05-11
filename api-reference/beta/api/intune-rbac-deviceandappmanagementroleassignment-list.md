---
title: Listar deviceAndAppManagementRoleAssignments
description: Lista propriedades e relações dos objetos deviceAndAppManagementRoleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 857312d76b2cb6a945b166aef2e45971b78271c3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899680"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="ce326-103">Listar deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="ce326-103">List deviceAndAppManagementRoleAssignments</span></span>

> <span data-ttu-id="ce326-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce326-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce326-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce326-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce326-106">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ce326-106">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce326-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ce326-107">Prerequisites</span></span>
<span data-ttu-id="ce326-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce326-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce326-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce326-110">Permission type</span></span>|<span data-ttu-id="ce326-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ce326-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce326-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce326-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce326-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce326-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="ce326-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce326-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce326-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce326-115">Not supported.</span></span>|
|<span data-ttu-id="ce326-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce326-116">Application</span></span>|<span data-ttu-id="ce326-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce326-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce326-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce326-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="ce326-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce326-119">Request headers</span></span>
|<span data-ttu-id="ce326-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ce326-120">Header</span></span>|<span data-ttu-id="ce326-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ce326-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce326-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce326-122">Authorization</span></span>|<span data-ttu-id="ce326-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce326-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce326-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ce326-124">Accept</span></span>|<span data-ttu-id="ce326-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce326-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce326-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce326-126">Request body</span></span>
<span data-ttu-id="ce326-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce326-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce326-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce326-128">Response</span></span>
<span data-ttu-id="ce326-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce326-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce326-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce326-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce326-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce326-131">Request</span></span>
<span data-ttu-id="ce326-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce326-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="ce326-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce326-133">Response</span></span>
<span data-ttu-id="ce326-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce326-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": [
    {
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
  ]
}
```




