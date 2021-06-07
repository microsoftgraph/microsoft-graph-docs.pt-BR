---
title: Listar deviceAndAppManagementRoleAssignments
description: Lista propriedades e relações dos objetos deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01a1c4c76a6340011437d3749abbdf8982d73b65
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756229"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="e9391-103">Listar deviceAndAppManagementRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="e9391-103">List deviceAndAppManagementRoleAssignments</span></span>

<span data-ttu-id="e9391-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9391-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9391-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9391-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9391-106">Lista propriedades e relações dos objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e9391-106">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9391-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9391-107">Prerequisites</span></span>
<span data-ttu-id="e9391-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9391-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9391-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9391-110">Permission type</span></span>|<span data-ttu-id="e9391-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9391-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9391-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9391-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9391-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9391-113">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="e9391-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9391-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9391-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9391-115">Not supported.</span></span>|
|<span data-ttu-id="e9391-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9391-116">Application</span></span>|<span data-ttu-id="e9391-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9391-117">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9391-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9391-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="e9391-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9391-119">Request headers</span></span>
|<span data-ttu-id="e9391-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9391-120">Header</span></span>|<span data-ttu-id="e9391-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e9391-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9391-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9391-122">Authorization</span></span>|<span data-ttu-id="e9391-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9391-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9391-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9391-124">Accept</span></span>|<span data-ttu-id="e9391-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e9391-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9391-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9391-126">Request body</span></span>
<span data-ttu-id="e9391-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9391-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9391-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9391-128">Response</span></span>
<span data-ttu-id="e9391-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9391-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9391-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9391-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9391-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9391-131">Request</span></span>
<span data-ttu-id="e9391-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9391-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="e9391-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9391-133">Response</span></span>
<span data-ttu-id="e9391-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9391-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




