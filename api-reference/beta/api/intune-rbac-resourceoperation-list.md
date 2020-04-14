---
title: Listar resourceOperations
description: Listar propriedades e relações dos objetos resourceOperation.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd783dbe77e0f5b0b81d5871ff97740eb792cdf8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455429"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="f93eb-103">Listar resourceOperations</span><span class="sxs-lookup"><span data-stu-id="f93eb-103">List resourceOperations</span></span>

<span data-ttu-id="f93eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f93eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f93eb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f93eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f93eb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f93eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f93eb-107">Listar propriedades e relações dos objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="f93eb-107">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f93eb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f93eb-108">Prerequisites</span></span>
<span data-ttu-id="f93eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f93eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f93eb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f93eb-111">Permission type</span></span>|<span data-ttu-id="f93eb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f93eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f93eb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f93eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f93eb-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f93eb-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="f93eb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f93eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f93eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f93eb-116">Not supported.</span></span>|
|<span data-ttu-id="f93eb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f93eb-117">Application</span></span>|<span data-ttu-id="f93eb-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f93eb-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f93eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f93eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="f93eb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f93eb-120">Request headers</span></span>
|<span data-ttu-id="f93eb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f93eb-121">Header</span></span>|<span data-ttu-id="f93eb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f93eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f93eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f93eb-123">Authorization</span></span>|<span data-ttu-id="f93eb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f93eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f93eb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f93eb-125">Accept</span></span>|<span data-ttu-id="f93eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f93eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f93eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f93eb-127">Request body</span></span>
<span data-ttu-id="f93eb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f93eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f93eb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f93eb-129">Response</span></span>
<span data-ttu-id="f93eb-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f93eb-130">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f93eb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f93eb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f93eb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f93eb-132">Request</span></span>
<span data-ttu-id="f93eb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f93eb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="f93eb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f93eb-134">Response</span></span>
<span data-ttu-id="f93eb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f93eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.resourceOperation",
      "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
      "resource": "Resource value",
      "resourceName": "Resource Name value",
      "actionName": "Action Name value",
      "description": "Description value",
      "enabledForScopeValidation": true
    }
  ]
}
```



