---
title: Criar roleScopeTag
description: Criar um novo objeto roleScopeTag.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b974205746ab7e50ceff1dd10de2238e1d8ab624
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955158"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="b6854-103">Criar roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="b6854-103">Create roleScopeTag</span></span>

> <span data-ttu-id="b6854-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6854-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6854-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6854-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6854-106">Criar um novo objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="b6854-106">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6854-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6854-107">Prerequisites</span></span>
<span data-ttu-id="b6854-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6854-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6854-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6854-110">Permission type</span></span>|<span data-ttu-id="b6854-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6854-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6854-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6854-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6854-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6854-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b6854-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6854-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6854-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6854-115">Not supported.</span></span>|
|<span data-ttu-id="b6854-116">Application</span><span class="sxs-lookup"><span data-stu-id="b6854-116">Application</span></span>|<span data-ttu-id="b6854-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6854-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6854-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6854-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="b6854-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6854-119">Request headers</span></span>
|<span data-ttu-id="b6854-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6854-120">Header</span></span>|<span data-ttu-id="b6854-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b6854-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6854-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6854-122">Authorization</span></span>|<span data-ttu-id="b6854-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6854-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6854-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6854-124">Accept</span></span>|<span data-ttu-id="b6854-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6854-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6854-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6854-126">Request body</span></span>
<span data-ttu-id="b6854-127">No corpo da solicitação, forneça uma representação JSON do objeto roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="b6854-127">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="b6854-128">A tabela a seguir mostra as propriedades que são necessárias ao criar roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="b6854-128">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="b6854-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6854-129">Property</span></span>|<span data-ttu-id="b6854-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6854-130">Type</span></span>|<span data-ttu-id="b6854-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6854-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6854-132">id</span><span class="sxs-lookup"><span data-stu-id="b6854-132">id</span></span>|<span data-ttu-id="b6854-133">String</span><span class="sxs-lookup"><span data-stu-id="b6854-133">String</span></span>|<span data-ttu-id="b6854-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b6854-134">Key of the entity.</span></span> <span data-ttu-id="b6854-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="b6854-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b6854-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b6854-136">displayName</span></span>|<span data-ttu-id="b6854-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6854-137">String</span></span>|<span data-ttu-id="b6854-138">O nome de exibição ou amigável da marca de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="b6854-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="b6854-139">description</span><span class="sxs-lookup"><span data-stu-id="b6854-139">description</span></span>|<span data-ttu-id="b6854-140">String</span><span class="sxs-lookup"><span data-stu-id="b6854-140">String</span></span>|<span data-ttu-id="b6854-141">Descrição da marca de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="b6854-141">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="b6854-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="b6854-142">isBuiltIn</span></span>|<span data-ttu-id="b6854-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6854-143">Boolean</span></span>|<span data-ttu-id="b6854-144">Descrição da marca de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="b6854-144">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="b6854-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6854-145">Response</span></span>
<span data-ttu-id="b6854-146">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6854-146">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6854-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6854-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6854-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6854-148">Request</span></span>
<span data-ttu-id="b6854-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6854-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6854-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6854-150">Response</span></span>
<span data-ttu-id="b6854-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6854-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





