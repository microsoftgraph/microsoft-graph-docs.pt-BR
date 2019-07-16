---
title: ação getRoleScopeTagsById
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 303d2ad206a669ae10a6f289904699d8eeb2e826
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725831"
---
# <a name="getrolescopetagsbyid-action"></a><span data-ttu-id="a42c5-103">ação getRoleScopeTagsById</span><span class="sxs-lookup"><span data-stu-id="a42c5-103">getRoleScopeTagsById action</span></span>

> <span data-ttu-id="a42c5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a42c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a42c5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a42c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a42c5-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a42c5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a42c5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a42c5-107">Prerequisites</span></span>
<span data-ttu-id="a42c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a42c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a42c5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a42c5-110">Permission type</span></span>|<span data-ttu-id="a42c5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a42c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a42c5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a42c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a42c5-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a42c5-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a42c5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a42c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a42c5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a42c5-115">Not supported.</span></span>|
|<span data-ttu-id="a42c5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a42c5-116">Application</span></span>|<span data-ttu-id="a42c5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a42c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a42c5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a42c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/getRoleScopeTagsById
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/getRoleScopeTagsById
```

## <a name="request-headers"></a><span data-ttu-id="a42c5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a42c5-119">Request headers</span></span>
|<span data-ttu-id="a42c5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a42c5-120">Header</span></span>|<span data-ttu-id="a42c5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a42c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a42c5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a42c5-122">Authorization</span></span>|<span data-ttu-id="a42c5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a42c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a42c5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a42c5-124">Accept</span></span>|<span data-ttu-id="a42c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a42c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a42c5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a42c5-126">Request body</span></span>
<span data-ttu-id="a42c5-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a42c5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a42c5-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a42c5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a42c5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a42c5-129">Property</span></span>|<span data-ttu-id="a42c5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a42c5-130">Type</span></span>|<span data-ttu-id="a42c5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a42c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a42c5-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a42c5-132">roleScopeTagIds</span></span>|<span data-ttu-id="a42c5-133">String collection</span><span class="sxs-lookup"><span data-stu-id="a42c5-133">String collection</span></span>|<span data-ttu-id="a42c5-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a42c5-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a42c5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a42c5-135">Response</span></span>
<span data-ttu-id="a42c5-136">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e uma coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a42c5-136">If successful, this action returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a42c5-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a42c5-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a42c5-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a42c5-138">Request</span></span>
<span data-ttu-id="a42c5-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a42c5-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/getRoleScopeTagsById

Content-type: application/json
Content-length: 65

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="a42c5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a42c5-140">Response</span></span>
<span data-ttu-id="a42c5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a42c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 231

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```





