---
title: Atualizar roleScopeTag
description: Atualiza as propriedades de um objeto roleScopeTag.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3670850bb0a9b3907b02c3e48d893b35ce7fcbb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799206"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="12650-103">Atualizar roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="12650-103">Update roleScopeTag</span></span>

> <span data-ttu-id="12650-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12650-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12650-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12650-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12650-106">Atualiza as propriedades de um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="12650-106">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12650-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12650-107">Prerequisites</span></span>
<span data-ttu-id="12650-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12650-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12650-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12650-110">Permission type</span></span>|<span data-ttu-id="12650-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12650-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12650-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12650-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12650-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12650-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="12650-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12650-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12650-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12650-115">Not supported.</span></span>|
|<span data-ttu-id="12650-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12650-116">Application</span></span>|<span data-ttu-id="12650-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12650-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12650-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12650-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="12650-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12650-119">Request headers</span></span>
|<span data-ttu-id="12650-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12650-120">Header</span></span>|<span data-ttu-id="12650-121">Valor</span><span class="sxs-lookup"><span data-stu-id="12650-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12650-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="12650-122">Authorization</span></span>|<span data-ttu-id="12650-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12650-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12650-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12650-124">Accept</span></span>|<span data-ttu-id="12650-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12650-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12650-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12650-126">Request body</span></span>
<span data-ttu-id="12650-127">No corpo da solicitação, forneça uma representação JSON do objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="12650-127">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="12650-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="12650-128">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="12650-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12650-129">Property</span></span>|<span data-ttu-id="12650-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="12650-130">Type</span></span>|<span data-ttu-id="12650-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="12650-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12650-132">id</span><span class="sxs-lookup"><span data-stu-id="12650-132">id</span></span>|<span data-ttu-id="12650-133">String</span><span class="sxs-lookup"><span data-stu-id="12650-133">String</span></span>|<span data-ttu-id="12650-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="12650-134">Key of the entity.</span></span> <span data-ttu-id="12650-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="12650-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="12650-136">displayName</span><span class="sxs-lookup"><span data-stu-id="12650-136">displayName</span></span>|<span data-ttu-id="12650-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12650-137">String</span></span>|<span data-ttu-id="12650-138">O nome de exibição ou amigável da marca de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="12650-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="12650-139">description</span><span class="sxs-lookup"><span data-stu-id="12650-139">description</span></span>|<span data-ttu-id="12650-140">String</span><span class="sxs-lookup"><span data-stu-id="12650-140">String</span></span>|<span data-ttu-id="12650-141">Descrição da marca de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="12650-141">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="12650-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="12650-142">Response</span></span>
<span data-ttu-id="12650-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12650-143">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12650-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12650-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="12650-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12650-145">Request</span></span>
<span data-ttu-id="12650-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12650-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="12650-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="12650-147">Response</span></span>
<span data-ttu-id="12650-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12650-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





