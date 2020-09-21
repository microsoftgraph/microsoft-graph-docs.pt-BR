---
title: Listar roleAssignments
description: Listar propriedades e relações de objeto de roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd048cc2a7fb2898fbcdf894b6cae862dfe904a0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965831"
---
# <a name="list-roleassignments"></a><span data-ttu-id="07c1f-103">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="07c1f-103">List roleAssignments</span></span>

<span data-ttu-id="07c1f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07c1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07c1f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07c1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07c1f-106">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="07c1f-106">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07c1f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07c1f-107">Prerequisites</span></span>
<span data-ttu-id="07c1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07c1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07c1f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07c1f-110">Permission type</span></span>|<span data-ttu-id="07c1f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="07c1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07c1f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07c1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07c1f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="07c1f-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="07c1f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07c1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07c1f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07c1f-115">Not supported.</span></span>|
|<span data-ttu-id="07c1f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07c1f-116">Application</span></span>|<span data-ttu-id="07c1f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07c1f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07c1f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07c1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="07c1f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07c1f-119">Request headers</span></span>
|<span data-ttu-id="07c1f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07c1f-120">Header</span></span>|<span data-ttu-id="07c1f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="07c1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07c1f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="07c1f-122">Authorization</span></span>|<span data-ttu-id="07c1f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07c1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07c1f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07c1f-124">Accept</span></span>|<span data-ttu-id="07c1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07c1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07c1f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07c1f-126">Request body</span></span>
<span data-ttu-id="07c1f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07c1f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07c1f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="07c1f-128">Response</span></span>
<span data-ttu-id="07c1f-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07c1f-129">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07c1f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07c1f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="07c1f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07c1f-131">Request</span></span>
<span data-ttu-id="07c1f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07c1f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="07c1f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="07c1f-133">Response</span></span>
<span data-ttu-id="07c1f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07c1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleAssignment",
      "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
      "displayName": "Display Name value",
      "description": "Description value",
      "resourceScopes": [
        "Resource Scopes value"
      ]
    }
  ]
}
```









