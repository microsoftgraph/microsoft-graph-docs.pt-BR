---
title: Listar roleAssignments
description: Listar propriedades e relações de objeto de roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39b7c379c7c5c764732e2c5d24f62f0b236bded9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420925"
---
# <a name="list-roleassignments"></a><span data-ttu-id="abcf9-103">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="abcf9-103">List roleAssignments</span></span>

<span data-ttu-id="abcf9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abcf9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abcf9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abcf9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abcf9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abcf9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abcf9-107">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="abcf9-107">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abcf9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abcf9-108">Prerequisites</span></span>
<span data-ttu-id="abcf9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abcf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abcf9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abcf9-111">Permission type</span></span>|<span data-ttu-id="abcf9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abcf9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abcf9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abcf9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abcf9-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="abcf9-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="abcf9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abcf9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abcf9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abcf9-116">Not supported.</span></span>|
|<span data-ttu-id="abcf9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abcf9-117">Application</span></span>|<span data-ttu-id="abcf9-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="abcf9-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abcf9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abcf9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="abcf9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abcf9-120">Request headers</span></span>
|<span data-ttu-id="abcf9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abcf9-121">Header</span></span>|<span data-ttu-id="abcf9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="abcf9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abcf9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="abcf9-123">Authorization</span></span>|<span data-ttu-id="abcf9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abcf9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abcf9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abcf9-125">Accept</span></span>|<span data-ttu-id="abcf9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abcf9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abcf9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abcf9-127">Request body</span></span>
<span data-ttu-id="abcf9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="abcf9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abcf9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="abcf9-129">Response</span></span>
<span data-ttu-id="abcf9-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abcf9-130">If successful, this method returns a `200 OK` response code and a collection of [roleAssignment](../resources/intune-rbac-roleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abcf9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abcf9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="abcf9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abcf9-132">Request</span></span>
<span data-ttu-id="abcf9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abcf9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

### <a name="response"></a><span data-ttu-id="abcf9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="abcf9-134">Response</span></span>
<span data-ttu-id="abcf9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abcf9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 403

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleAssignment",
      "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
      "displayName": "Display Name value",
      "description": "Description value",
      "scopeMembers": [
        "Scope Members value"
      ],
      "scopeType": "allDevices",
      "resourceScopes": [
        "Resource Scopes value"
      ]
    }
  ]
}
```



