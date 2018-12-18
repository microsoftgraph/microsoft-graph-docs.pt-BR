---
title: Excluir deviceAndAppManagementRoleAssignment
description: Exclui deviceAndAppManagementRoleAssignment.
author: tfitzmac
ms.openlocfilehash: cccc4f95d21b4db8e9275ae5b6c2225bdbdce53d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346078"
---
# <a name="delete-deviceandappmanagementroleassignment"></a><span data-ttu-id="e1bb5-103">Excluir deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e1bb5-103">Delete deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="e1bb5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e1bb5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1bb5-105">Exclui [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e1bb5-105">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1bb5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1bb5-106">Prerequisites</span></span>
<span data-ttu-id="e1bb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1bb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1bb5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1bb5-109">Permission type</span></span>|<span data-ttu-id="e1bb5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1bb5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1bb5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1bb5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1bb5-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1bb5-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="e1bb5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1bb5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1bb5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1bb5-114">Not supported.</span></span>|
|<span data-ttu-id="e1bb5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1bb5-115">Application</span></span>|<span data-ttu-id="e1bb5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1bb5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1bb5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1bb5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e1bb5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1bb5-118">Request headers</span></span>
|<span data-ttu-id="e1bb5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1bb5-119">Header</span></span>|<span data-ttu-id="e1bb5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e1bb5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1bb5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1bb5-121">Authorization</span></span>|<span data-ttu-id="e1bb5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1bb5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1bb5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e1bb5-123">Accept</span></span>|<span data-ttu-id="e1bb5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e1bb5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1bb5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1bb5-125">Request body</span></span>
<span data-ttu-id="e1bb5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1bb5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1bb5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1bb5-127">Response</span></span>
<span data-ttu-id="e1bb5-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e1bb5-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e1bb5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1bb5-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1bb5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1bb5-130">Request</span></span>
<span data-ttu-id="e1bb5-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1bb5-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e1bb5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1bb5-132">Response</span></span>
<span data-ttu-id="e1bb5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1bb5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



