---
title: atribuir ação
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c2f1825da70c7e708066d4b5fed2282ccfef32a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801611"
---
# <a name="assign-action"></a><span data-ttu-id="d03e7-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="d03e7-103">assign action</span></span>

> <span data-ttu-id="d03e7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d03e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d03e7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d03e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d03e7-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d03e7-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d03e7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d03e7-107">Prerequisites</span></span>
<span data-ttu-id="d03e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d03e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d03e7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d03e7-110">Permission type</span></span>|<span data-ttu-id="d03e7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d03e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d03e7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d03e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d03e7-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d03e7-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d03e7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d03e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d03e7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d03e7-115">Not supported.</span></span>|
|<span data-ttu-id="d03e7-116">Application</span><span class="sxs-lookup"><span data-stu-id="d03e7-116">Application</span></span>|<span data-ttu-id="d03e7-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d03e7-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d03e7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d03e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/{roleScopeTagId}/assign
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d03e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d03e7-119">Request headers</span></span>
|<span data-ttu-id="d03e7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d03e7-120">Header</span></span>|<span data-ttu-id="d03e7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d03e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d03e7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d03e7-122">Authorization</span></span>|<span data-ttu-id="d03e7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d03e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d03e7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d03e7-124">Accept</span></span>|<span data-ttu-id="d03e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d03e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d03e7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d03e7-126">Request body</span></span>
<span data-ttu-id="d03e7-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d03e7-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d03e7-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d03e7-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d03e7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d03e7-129">Property</span></span>|<span data-ttu-id="d03e7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d03e7-130">Type</span></span>|<span data-ttu-id="d03e7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d03e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d03e7-132">assignments</span><span class="sxs-lookup"><span data-stu-id="d03e7-132">assignments</span></span>|<span data-ttu-id="d03e7-133">coleção [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d03e7-133">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="d03e7-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d03e7-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d03e7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d03e7-135">Response</span></span>
<span data-ttu-id="d03e7-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d03e7-136">If successful, this action returns a `200 OK` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d03e7-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d03e7-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d03e7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d03e7-138">Request</span></span>
<span data-ttu-id="d03e7-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d03e7-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}/assign

Content-type: application/json
Content-length: 274

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d03e7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d03e7-140">Response</span></span>
<span data-ttu-id="d03e7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d03e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




