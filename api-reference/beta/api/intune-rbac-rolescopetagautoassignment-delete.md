---
title: Excluir roleScopeTagAutoAssignment
description: Exclui um roleScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27ce42f45f1c749933557258a5cc53f8341f5ca5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134498"
---
# <a name="delete-rolescopetagautoassignment"></a><span data-ttu-id="3fd71-103">Excluir roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="3fd71-103">Delete roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="3fd71-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fd71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3fd71-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3fd71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fd71-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3fd71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fd71-107">Exclui um [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3fd71-107">Deletes a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fd71-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3fd71-108">Prerequisites</span></span>
<span data-ttu-id="3fd71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fd71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fd71-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fd71-111">Permission type</span></span>|<span data-ttu-id="3fd71-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3fd71-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fd71-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fd71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fd71-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fd71-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3fd71-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fd71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fd71-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fd71-116">Not supported.</span></span>|
|<span data-ttu-id="3fd71-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fd71-117">Application</span></span>|<span data-ttu-id="3fd71-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fd71-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fd71-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fd71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3fd71-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fd71-120">Request headers</span></span>
|<span data-ttu-id="3fd71-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3fd71-121">Header</span></span>|<span data-ttu-id="3fd71-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3fd71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fd71-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fd71-123">Authorization</span></span>|<span data-ttu-id="3fd71-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fd71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fd71-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3fd71-125">Accept</span></span>|<span data-ttu-id="3fd71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fd71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fd71-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fd71-127">Request body</span></span>
<span data-ttu-id="3fd71-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3fd71-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fd71-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fd71-129">Response</span></span>
<span data-ttu-id="3fd71-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3fd71-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3fd71-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fd71-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fd71-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fd71-132">Request</span></span>
<span data-ttu-id="3fd71-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fd71-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

### <a name="response"></a><span data-ttu-id="3fd71-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fd71-134">Response</span></span>
<span data-ttu-id="3fd71-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3fd71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




