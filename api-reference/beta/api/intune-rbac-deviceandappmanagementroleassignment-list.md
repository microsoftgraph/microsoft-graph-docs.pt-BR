---
title: Listar deviceAndAppManagementRoleAssignments
description: Lista propriedades e relações dos objetos deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d1766616f2166fc7cbf50b304053a3d96c81d865
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044974"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="f4bdd-103">Listar deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="f4bdd-103">List deviceAndAppManagementRoleAssignments</span></span>

<span data-ttu-id="f4bdd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4bdd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4bdd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4bdd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4bdd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4bdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4bdd-107">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f4bdd-107">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4bdd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4bdd-108">Prerequisites</span></span>
<span data-ttu-id="f4bdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4bdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4bdd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4bdd-111">Permission type</span></span>|<span data-ttu-id="f4bdd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4bdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4bdd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4bdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4bdd-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4bdd-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="f4bdd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4bdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4bdd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4bdd-116">Not supported.</span></span>|
|<span data-ttu-id="f4bdd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4bdd-117">Application</span></span>|<span data-ttu-id="f4bdd-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4bdd-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4bdd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4bdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="f4bdd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4bdd-120">Request headers</span></span>
|<span data-ttu-id="f4bdd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4bdd-121">Header</span></span>|<span data-ttu-id="f4bdd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f4bdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4bdd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4bdd-123">Authorization</span></span>|<span data-ttu-id="f4bdd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4bdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4bdd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4bdd-125">Accept</span></span>|<span data-ttu-id="f4bdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4bdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4bdd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4bdd-127">Request body</span></span>
<span data-ttu-id="f4bdd-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f4bdd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4bdd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4bdd-129">Response</span></span>
<span data-ttu-id="f4bdd-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4bdd-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4bdd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4bdd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4bdd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4bdd-132">Request</span></span>
<span data-ttu-id="f4bdd-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4bdd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="f4bdd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4bdd-134">Response</span></span>
<span data-ttu-id="f4bdd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4bdd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






