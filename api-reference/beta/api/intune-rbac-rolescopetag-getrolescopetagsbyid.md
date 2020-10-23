---
title: ação getRoleScopeTagsById
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9b814ec665ec7ef590d05deec697b46376ffa1b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706349"
---
# <a name="getrolescopetagsbyid-action"></a><span data-ttu-id="0db4a-103">ação getRoleScopeTagsById</span><span class="sxs-lookup"><span data-stu-id="0db4a-103">getRoleScopeTagsById action</span></span>

<span data-ttu-id="0db4a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0db4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0db4a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0db4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0db4a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0db4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0db4a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0db4a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0db4a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0db4a-108">Prerequisites</span></span>
<span data-ttu-id="0db4a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0db4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0db4a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0db4a-111">Permission type</span></span>|<span data-ttu-id="0db4a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0db4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0db4a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0db4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0db4a-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0db4a-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="0db4a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0db4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0db4a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0db4a-116">Not supported.</span></span>|
|<span data-ttu-id="0db4a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0db4a-117">Application</span></span>|<span data-ttu-id="0db4a-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0db4a-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0db4a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0db4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/getRoleScopeTagsById
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/getRoleScopeTagsById
```

## <a name="request-headers"></a><span data-ttu-id="0db4a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0db4a-120">Request headers</span></span>
|<span data-ttu-id="0db4a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0db4a-121">Header</span></span>|<span data-ttu-id="0db4a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0db4a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0db4a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0db4a-123">Authorization</span></span>|<span data-ttu-id="0db4a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0db4a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0db4a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0db4a-125">Accept</span></span>|<span data-ttu-id="0db4a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0db4a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0db4a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0db4a-127">Request body</span></span>
<span data-ttu-id="0db4a-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0db4a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0db4a-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0db4a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0db4a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0db4a-130">Property</span></span>|<span data-ttu-id="0db4a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0db4a-131">Type</span></span>|<span data-ttu-id="0db4a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0db4a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0db4a-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0db4a-133">roleScopeTagIds</span></span>|<span data-ttu-id="0db4a-134">String collection</span><span class="sxs-lookup"><span data-stu-id="0db4a-134">String collection</span></span>|<span data-ttu-id="0db4a-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0db4a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0db4a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0db4a-136">Response</span></span>
<span data-ttu-id="0db4a-137">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e uma coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0db4a-137">If successful, this action returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0db4a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0db4a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0db4a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0db4a-139">Request</span></span>
<span data-ttu-id="0db4a-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0db4a-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0db4a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0db4a-141">Response</span></span>
<span data-ttu-id="0db4a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0db4a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value",
      "isBuiltIn": true
    }
  ]
}
```





