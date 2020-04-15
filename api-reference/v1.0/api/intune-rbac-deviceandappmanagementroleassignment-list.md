---
title: Listar deviceAndAppManagementRoleAssignments
description: Lista propriedades e relações dos objetos deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cf69a056bf57a0374e894ce312c2dc3a0bc22437
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452727"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="87182-103">Listar deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="87182-103">List deviceAndAppManagementRoleAssignments</span></span>

<span data-ttu-id="87182-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87182-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87182-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87182-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87182-106">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="87182-106">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87182-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87182-107">Prerequisites</span></span>
<span data-ttu-id="87182-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87182-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87182-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87182-110">Permission type</span></span>|<span data-ttu-id="87182-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87182-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87182-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87182-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87182-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="87182-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="87182-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87182-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87182-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87182-115">Not supported.</span></span>|
|<span data-ttu-id="87182-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87182-116">Application</span></span>|<span data-ttu-id="87182-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87182-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87182-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87182-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="87182-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87182-119">Request headers</span></span>
|<span data-ttu-id="87182-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87182-120">Header</span></span>|<span data-ttu-id="87182-121">Valor</span><span class="sxs-lookup"><span data-stu-id="87182-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87182-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="87182-122">Authorization</span></span>|<span data-ttu-id="87182-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87182-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87182-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87182-124">Accept</span></span>|<span data-ttu-id="87182-125">application/json</span><span class="sxs-lookup"><span data-stu-id="87182-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87182-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87182-126">Request body</span></span>
<span data-ttu-id="87182-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87182-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87182-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="87182-128">Response</span></span>
<span data-ttu-id="87182-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87182-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87182-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87182-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="87182-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87182-131">Request</span></span>
<span data-ttu-id="87182-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87182-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="87182-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="87182-133">Response</span></span>
<span data-ttu-id="87182-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87182-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






