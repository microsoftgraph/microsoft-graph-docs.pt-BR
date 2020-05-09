---
title: Listar roleScopeTagAutoAssignments
description: Listar Propriedades e relações dos objetos roleScopeTagAutoAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7582a2c7f785060af2f739fcf8ae7cacb1431e3d
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177293"
---
# <a name="list-rolescopetagautoassignments"></a><span data-ttu-id="62e4c-103">Listar roleScopeTagAutoAssignments</span><span class="sxs-lookup"><span data-stu-id="62e4c-103">List roleScopeTagAutoAssignments</span></span>

<span data-ttu-id="62e4c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62e4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62e4c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62e4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62e4c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62e4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62e4c-107">Listar Propriedades e relações dos objetos [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="62e4c-107">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62e4c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62e4c-108">Prerequisites</span></span>
<span data-ttu-id="62e4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62e4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62e4c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62e4c-111">Permission type</span></span>|<span data-ttu-id="62e4c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62e4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62e4c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62e4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62e4c-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="62e4c-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="62e4c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62e4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62e4c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62e4c-116">Not supported.</span></span>|
|<span data-ttu-id="62e4c-117">Application</span><span class="sxs-lookup"><span data-stu-id="62e4c-117">Application</span></span>|<span data-ttu-id="62e4c-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="62e4c-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62e4c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62e4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="62e4c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62e4c-120">Request headers</span></span>
|<span data-ttu-id="62e4c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62e4c-121">Header</span></span>|<span data-ttu-id="62e4c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="62e4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62e4c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62e4c-123">Authorization</span></span>|<span data-ttu-id="62e4c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62e4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62e4c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62e4c-125">Accept</span></span>|<span data-ttu-id="62e4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62e4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62e4c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62e4c-127">Request body</span></span>
<span data-ttu-id="62e4c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62e4c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62e4c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="62e4c-129">Response</span></span>
<span data-ttu-id="62e4c-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62e4c-130">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62e4c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62e4c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="62e4c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62e4c-132">Request</span></span>
<span data-ttu-id="62e4c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62e4c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

### <a name="response"></a><span data-ttu-id="62e4c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="62e4c-134">Response</span></span>
<span data-ttu-id="62e4c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62e4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```



