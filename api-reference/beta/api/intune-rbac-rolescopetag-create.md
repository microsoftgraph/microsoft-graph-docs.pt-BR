---
title: Criar roleScopeTag
description: Crie um novo objeto roleScopeTag.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7d02eb907ee0fbedde3240906277601eca8601e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156664"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="0bade-103">Criar roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0bade-103">Create roleScopeTag</span></span>

<span data-ttu-id="0bade-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bade-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bade-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0bade-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bade-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0bade-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bade-107">Crie um novo [objeto roleScopeTag.](../resources/intune-rbac-rolescopetag.md)</span><span class="sxs-lookup"><span data-stu-id="0bade-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bade-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0bade-108">Prerequisites</span></span>
<span data-ttu-id="0bade-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bade-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bade-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bade-111">Permission type</span></span>|<span data-ttu-id="0bade-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0bade-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bade-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bade-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bade-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bade-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0bade-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bade-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bade-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bade-116">Not supported.</span></span>|
|<span data-ttu-id="0bade-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bade-117">Application</span></span>|<span data-ttu-id="0bade-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bade-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bade-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bade-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="0bade-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bade-120">Request headers</span></span>
|<span data-ttu-id="0bade-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0bade-121">Header</span></span>|<span data-ttu-id="0bade-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0bade-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bade-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bade-123">Authorization</span></span>|<span data-ttu-id="0bade-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bade-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bade-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0bade-125">Accept</span></span>|<span data-ttu-id="0bade-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bade-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bade-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bade-127">Request body</span></span>
<span data-ttu-id="0bade-128">No corpo da solicitação, fornece uma representação JSON para o objeto roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="0bade-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="0bade-129">A tabela a seguir mostra as propriedades que são necessárias ao criar a roleScopeTag.</span><span class="sxs-lookup"><span data-stu-id="0bade-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="0bade-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bade-130">Property</span></span>|<span data-ttu-id="0bade-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bade-131">Type</span></span>|<span data-ttu-id="0bade-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bade-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bade-133">id</span><span class="sxs-lookup"><span data-stu-id="0bade-133">id</span></span>|<span data-ttu-id="0bade-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bade-134">String</span></span>|<span data-ttu-id="0bade-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0bade-135">Key of the entity.</span></span> <span data-ttu-id="0bade-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0bade-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="0bade-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0bade-137">displayName</span></span>|<span data-ttu-id="0bade-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bade-138">String</span></span>|<span data-ttu-id="0bade-139">O nome de exibição ou amigável da Marca de Escopo de Função.</span><span class="sxs-lookup"><span data-stu-id="0bade-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="0bade-140">descrição</span><span class="sxs-lookup"><span data-stu-id="0bade-140">description</span></span>|<span data-ttu-id="0bade-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bade-141">String</span></span>|<span data-ttu-id="0bade-142">Descrição da marca escopo de função.</span><span class="sxs-lookup"><span data-stu-id="0bade-142">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="0bade-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="0bade-143">isBuiltIn</span></span>|<span data-ttu-id="0bade-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="0bade-144">Boolean</span></span>|<span data-ttu-id="0bade-145">Descrição da marca escopo de função.</span><span class="sxs-lookup"><span data-stu-id="0bade-145">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="0bade-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bade-146">Response</span></span>
<span data-ttu-id="0bade-147">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bade-147">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bade-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bade-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bade-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bade-149">Request</span></span>
<span data-ttu-id="0bade-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bade-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0bade-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bade-151">Response</span></span>
<span data-ttu-id="0bade-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bade-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




