---
title: Criar roleScopeTag
description: Criar um novo objeto roleScopeTag.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 248f92bc6eaa757a69c20b2a9c684d4873b9dae6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304679"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="33737-103">Criar roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="33737-103">Create roleScopeTag</span></span>

<span data-ttu-id="33737-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33737-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33737-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33737-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33737-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33737-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33737-107">Criar um novo objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="33737-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33737-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33737-108">Prerequisites</span></span>
<span data-ttu-id="33737-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33737-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33737-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33737-111">Permission type</span></span>|<span data-ttu-id="33737-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33737-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33737-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33737-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33737-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33737-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="33737-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33737-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33737-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33737-116">Not supported.</span></span>|
|<span data-ttu-id="33737-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33737-117">Application</span></span>|<span data-ttu-id="33737-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33737-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33737-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33737-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="33737-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33737-120">Request headers</span></span>
|<span data-ttu-id="33737-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33737-121">Header</span></span>|<span data-ttu-id="33737-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33737-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33737-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33737-123">Authorization</span></span>|<span data-ttu-id="33737-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33737-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33737-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33737-125">Accept</span></span>|<span data-ttu-id="33737-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33737-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33737-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33737-127">Request body</span></span>
<span data-ttu-id="33737-128">No corpo da solicitação, forneça uma representação JSON do objeto roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="33737-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="33737-129">A tabela a seguir mostra as propriedades que são necessárias ao criar roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="33737-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="33737-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33737-130">Property</span></span>|<span data-ttu-id="33737-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="33737-131">Type</span></span>|<span data-ttu-id="33737-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="33737-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33737-133">id</span><span class="sxs-lookup"><span data-stu-id="33737-133">id</span></span>|<span data-ttu-id="33737-134">String</span><span class="sxs-lookup"><span data-stu-id="33737-134">String</span></span>|<span data-ttu-id="33737-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="33737-135">Key of the entity.</span></span> <span data-ttu-id="33737-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="33737-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="33737-137">displayName</span><span class="sxs-lookup"><span data-stu-id="33737-137">displayName</span></span>|<span data-ttu-id="33737-138">String</span><span class="sxs-lookup"><span data-stu-id="33737-138">String</span></span>|<span data-ttu-id="33737-139">O nome de exibição ou amigável da marca de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="33737-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="33737-140">description</span><span class="sxs-lookup"><span data-stu-id="33737-140">description</span></span>|<span data-ttu-id="33737-141">String</span><span class="sxs-lookup"><span data-stu-id="33737-141">String</span></span>|<span data-ttu-id="33737-142">Descrição da marca de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="33737-142">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="33737-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="33737-143">isBuiltIn</span></span>|<span data-ttu-id="33737-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="33737-144">Boolean</span></span>|<span data-ttu-id="33737-145">Descrição da marca de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="33737-145">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="33737-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="33737-146">Response</span></span>
<span data-ttu-id="33737-147">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33737-147">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33737-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33737-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="33737-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33737-149">Request</span></span>
<span data-ttu-id="33737-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33737-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value",
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="33737-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="33737-151">Response</span></span>
<span data-ttu-id="33737-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33737-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 204

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value",
  "isBuiltIn": true
}
```




