---
title: Excluir roleScopeTagAutoAssignment
description: Exclui roleScopeTagAutoAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6321361994a16fdd4b3a2633793ec8f8f2cbb61d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002424"
---
# <a name="delete-rolescopetagautoassignment"></a><span data-ttu-id="603ea-103">Excluir roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="603ea-103">Delete roleScopeTagAutoAssignment</span></span>

> <span data-ttu-id="603ea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="603ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="603ea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="603ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="603ea-106">Exclui [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span><span class="sxs-lookup"><span data-stu-id="603ea-106">Deletes a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="603ea-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="603ea-107">Prerequisites</span></span>
<span data-ttu-id="603ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="603ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="603ea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="603ea-110">Permission type</span></span>|<span data-ttu-id="603ea-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="603ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="603ea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="603ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="603ea-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="603ea-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="603ea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="603ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="603ea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="603ea-115">Not supported.</span></span>|
|<span data-ttu-id="603ea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="603ea-116">Application</span></span>|<span data-ttu-id="603ea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="603ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="603ea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="603ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="603ea-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="603ea-119">Request headers</span></span>
|<span data-ttu-id="603ea-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="603ea-120">Header</span></span>|<span data-ttu-id="603ea-121">Valor</span><span class="sxs-lookup"><span data-stu-id="603ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="603ea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="603ea-122">Authorization</span></span>|<span data-ttu-id="603ea-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="603ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="603ea-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="603ea-124">Accept</span></span>|<span data-ttu-id="603ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="603ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="603ea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="603ea-126">Request body</span></span>
<span data-ttu-id="603ea-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="603ea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="603ea-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="603ea-128">Response</span></span>
<span data-ttu-id="603ea-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="603ea-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="603ea-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="603ea-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="603ea-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="603ea-131">Request</span></span>
<span data-ttu-id="603ea-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="603ea-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

### <a name="response"></a><span data-ttu-id="603ea-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="603ea-133">Response</span></span>
<span data-ttu-id="603ea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="603ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





