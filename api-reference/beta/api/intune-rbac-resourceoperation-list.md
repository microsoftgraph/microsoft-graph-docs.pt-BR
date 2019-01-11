---
title: Listar resourceOperations
description: Listar propriedades e relações dos objetos resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 524a92296febd521dae55289ac8a4ca7ddea7da3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835312"
---
# <a name="list-resourceoperations"></a><span data-ttu-id="99cbe-103">Listar resourceOperations</span><span class="sxs-lookup"><span data-stu-id="99cbe-103">List resourceOperations</span></span>

> <span data-ttu-id="99cbe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99cbe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99cbe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99cbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99cbe-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="99cbe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99cbe-107">Listar propriedades e relações dos objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="99cbe-107">List properties and relationships of the [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99cbe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99cbe-108">Prerequisites</span></span>
<span data-ttu-id="99cbe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99cbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99cbe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99cbe-111">Permission type</span></span>|<span data-ttu-id="99cbe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99cbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99cbe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99cbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99cbe-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="99cbe-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="99cbe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99cbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99cbe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99cbe-116">Not supported.</span></span>|
|<span data-ttu-id="99cbe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99cbe-117">Application</span></span>|<span data-ttu-id="99cbe-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99cbe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99cbe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99cbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="99cbe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99cbe-120">Request headers</span></span>
|<span data-ttu-id="99cbe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99cbe-121">Header</span></span>|<span data-ttu-id="99cbe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="99cbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99cbe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="99cbe-123">Authorization</span></span>|<span data-ttu-id="99cbe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99cbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99cbe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99cbe-125">Accept</span></span>|<span data-ttu-id="99cbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99cbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99cbe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99cbe-127">Request body</span></span>
<span data-ttu-id="99cbe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99cbe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99cbe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="99cbe-129">Response</span></span>
<span data-ttu-id="99cbe-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [resourceOperation](../resources/intune-rbac-resourceoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99cbe-130">If successful, this method returns a `200 OK` response code and a collection of [resourceOperation](../resources/intune-rbac-resourceoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99cbe-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99cbe-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="99cbe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99cbe-132">Request</span></span>
<span data-ttu-id="99cbe-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99cbe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations
```

### <a name="response"></a><span data-ttu-id="99cbe-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="99cbe-134">Response</span></span>
<span data-ttu-id="99cbe-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99cbe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





