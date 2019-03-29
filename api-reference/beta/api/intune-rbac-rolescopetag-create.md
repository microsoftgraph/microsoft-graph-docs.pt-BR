---
title: Criar roleScopeTag
description: Criar um novo objeto roleScopeTag.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbdc7089dc7f02fc49610e3feab07105a83c5984
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959450"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="f32b9-103">Criar roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="f32b9-103">Create roleScopeTag</span></span>

> <span data-ttu-id="f32b9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f32b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f32b9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f32b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f32b9-106">Criar um novo objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="f32b9-106">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f32b9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f32b9-107">Prerequisites</span></span>
<span data-ttu-id="f32b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f32b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f32b9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f32b9-110">Permission type</span></span>|<span data-ttu-id="f32b9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f32b9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f32b9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f32b9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f32b9-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f32b9-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f32b9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f32b9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f32b9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f32b9-115">Not supported.</span></span>|
|<span data-ttu-id="f32b9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f32b9-116">Application</span></span>|<span data-ttu-id="f32b9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f32b9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f32b9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f32b9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="f32b9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f32b9-119">Request headers</span></span>
|<span data-ttu-id="f32b9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f32b9-120">Header</span></span>|<span data-ttu-id="f32b9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f32b9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f32b9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f32b9-122">Authorization</span></span>|<span data-ttu-id="f32b9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f32b9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f32b9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f32b9-124">Accept</span></span>|<span data-ttu-id="f32b9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f32b9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f32b9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f32b9-126">Request body</span></span>
<span data-ttu-id="f32b9-127">No corpo da solicitação, forneça uma representação JSON do objeto roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="f32b9-127">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="f32b9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="f32b9-128">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="f32b9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f32b9-129">Property</span></span>|<span data-ttu-id="f32b9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f32b9-130">Type</span></span>|<span data-ttu-id="f32b9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f32b9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f32b9-132">id</span><span class="sxs-lookup"><span data-stu-id="f32b9-132">id</span></span>|<span data-ttu-id="f32b9-133">String</span><span class="sxs-lookup"><span data-stu-id="f32b9-133">String</span></span>|<span data-ttu-id="f32b9-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f32b9-134">Key of the entity.</span></span> <span data-ttu-id="f32b9-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="f32b9-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="f32b9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f32b9-136">displayName</span></span>|<span data-ttu-id="f32b9-137">String</span><span class="sxs-lookup"><span data-stu-id="f32b9-137">String</span></span>|<span data-ttu-id="f32b9-138">O nome de exibição ou amigável da marca de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="f32b9-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="f32b9-139">descrição</span><span class="sxs-lookup"><span data-stu-id="f32b9-139">description</span></span>|<span data-ttu-id="f32b9-140">String</span><span class="sxs-lookup"><span data-stu-id="f32b9-140">String</span></span>|<span data-ttu-id="f32b9-141">Descrição da marca de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="f32b9-141">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="f32b9-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f32b9-142">Response</span></span>
<span data-ttu-id="f32b9-143">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f32b9-143">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f32b9-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f32b9-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="f32b9-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f32b9-145">Request</span></span>
<span data-ttu-id="f32b9-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f32b9-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="f32b9-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="f32b9-147">Response</span></span>
<span data-ttu-id="f32b9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f32b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```




