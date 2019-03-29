---
title: Excluir deviceAndAppManagementRoleDefinition
description: Exclui deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ddd1be965bc860e18633cca38165927486db1ed
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979386"
---
# <a name="delete-deviceandappmanagementroledefinition"></a><span data-ttu-id="aee00-103">Excluir deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="aee00-103">Delete deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="aee00-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aee00-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aee00-105">Exclui [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="aee00-105">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aee00-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aee00-106">Prerequisites</span></span>
<span data-ttu-id="aee00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aee00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aee00-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aee00-109">Permission type</span></span>|<span data-ttu-id="aee00-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aee00-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aee00-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aee00-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aee00-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee00-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="aee00-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aee00-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aee00-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aee00-114">Not supported.</span></span>|
|<span data-ttu-id="aee00-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aee00-115">Application</span></span>|<span data-ttu-id="aee00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aee00-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aee00-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aee00-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="aee00-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aee00-118">Request headers</span></span>
|<span data-ttu-id="aee00-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aee00-119">Header</span></span>|<span data-ttu-id="aee00-120">Valor</span><span class="sxs-lookup"><span data-stu-id="aee00-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aee00-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="aee00-121">Authorization</span></span>|<span data-ttu-id="aee00-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aee00-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aee00-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aee00-123">Accept</span></span>|<span data-ttu-id="aee00-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aee00-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aee00-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aee00-125">Request body</span></span>
<span data-ttu-id="aee00-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aee00-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aee00-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="aee00-127">Response</span></span>
<span data-ttu-id="aee00-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aee00-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aee00-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aee00-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="aee00-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aee00-130">Request</span></span>
<span data-ttu-id="aee00-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aee00-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="aee00-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="aee00-132">Response</span></span>
<span data-ttu-id="aee00-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aee00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



