---
title: Listar roleAssignments
description: Listar propriedades e relações de objeto de roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8b24d2942e50d5bc4de11e5e8c0fad6ffcf6809
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960311"
---
# <a name="list-roleassignments"></a><span data-ttu-id="ebd90-103">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="ebd90-103">List roleAssignments</span></span>

> <span data-ttu-id="ebd90-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebd90-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebd90-105">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ebd90-105">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebd90-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebd90-106">Prerequisites</span></span>
<span data-ttu-id="ebd90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebd90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebd90-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebd90-109">Permission type</span></span>|<span data-ttu-id="ebd90-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ebd90-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebd90-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebd90-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ebd90-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebd90-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="ebd90-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebd90-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebd90-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebd90-114">Not supported.</span></span>|
|<span data-ttu-id="ebd90-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebd90-115">Application</span></span>|<span data-ttu-id="ebd90-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebd90-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebd90-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebd90-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="ebd90-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd90-118">Request headers</span></span>
|<span data-ttu-id="ebd90-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebd90-119">Header</span></span>|<span data-ttu-id="ebd90-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ebd90-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebd90-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebd90-121">Authorization</span></span>|<span data-ttu-id="ebd90-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebd90-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebd90-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebd90-123">Accept</span></span>|<span data-ttu-id="ebd90-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ebd90-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebd90-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd90-125">Request body</span></span>
<span data-ttu-id="ebd90-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ebd90-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebd90-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebd90-127">Response</span></span>
<span data-ttu-id="ebd90-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebd90-128">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebd90-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebd90-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebd90-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd90-130">Request</span></span>
<span data-ttu-id="ebd90-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebd90-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="ebd90-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebd90-132">Response</span></span>
<span data-ttu-id="ebd90-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebd90-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



