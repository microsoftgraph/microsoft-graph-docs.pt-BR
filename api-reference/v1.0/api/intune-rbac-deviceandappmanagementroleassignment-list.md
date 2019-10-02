---
title: Listar deviceAndAppManagementRoleAssignments
description: Lista propriedades e relações dos objetos deviceAndAppManagementRoleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 088ed802195be45c7176ec026209412754f15223
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361984"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="246e0-103">Listar deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="246e0-103">List deviceAndAppManagementRoleAssignments</span></span>

> <span data-ttu-id="246e0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="246e0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="246e0-105">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="246e0-105">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="246e0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="246e0-106">Prerequisites</span></span>
<span data-ttu-id="246e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="246e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="246e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="246e0-109">Permission type</span></span>|<span data-ttu-id="246e0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="246e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="246e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="246e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="246e0-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="246e0-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="246e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="246e0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="246e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="246e0-114">Not supported.</span></span>|
|<span data-ttu-id="246e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="246e0-115">Application</span></span>|<span data-ttu-id="246e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="246e0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="246e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="246e0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="246e0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="246e0-118">Request headers</span></span>
|<span data-ttu-id="246e0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="246e0-119">Header</span></span>|<span data-ttu-id="246e0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="246e0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="246e0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="246e0-121">Authorization</span></span>|<span data-ttu-id="246e0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="246e0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="246e0-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="246e0-123">Accept</span></span>|<span data-ttu-id="246e0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="246e0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="246e0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="246e0-125">Request body</span></span>
<span data-ttu-id="246e0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="246e0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="246e0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="246e0-127">Response</span></span>
<span data-ttu-id="246e0-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="246e0-128">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="246e0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="246e0-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="246e0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="246e0-130">Request</span></span>
<span data-ttu-id="246e0-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="246e0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="246e0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="246e0-132">Response</span></span>
<span data-ttu-id="246e0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="246e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "value": [
    {
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
  ]
}
```




