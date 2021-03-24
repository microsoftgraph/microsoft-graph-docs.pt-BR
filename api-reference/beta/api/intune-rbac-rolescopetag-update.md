---
title: Atualizar roleScopeTag
description: Atualize as propriedades de um objeto roleScopeTag.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56ba0645b7aff34a7902417f15ab40f75c07c1a9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141509"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="3b8d7-103">Atualizar roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3b8d7-103">Update roleScopeTag</span></span>

<span data-ttu-id="3b8d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b8d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b8d7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b8d7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b8d7-107">Atualize as propriedades de um [objeto roleScopeTag.](../resources/intune-rbac-rolescopetag.md)</span><span class="sxs-lookup"><span data-stu-id="3b8d7-107">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b8d7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b8d7-108">Prerequisites</span></span>
<span data-ttu-id="3b8d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b8d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b8d7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b8d7-111">Permission type</span></span>|<span data-ttu-id="3b8d7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b8d7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b8d7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b8d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b8d7-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b8d7-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3b8d7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b8d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b8d7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-116">Not supported.</span></span>|
|<span data-ttu-id="3b8d7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b8d7-117">Application</span></span>|<span data-ttu-id="3b8d7-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b8d7-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b8d7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b8d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="3b8d7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b8d7-120">Request headers</span></span>
|<span data-ttu-id="3b8d7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b8d7-121">Header</span></span>|<span data-ttu-id="3b8d7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3b8d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b8d7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b8d7-123">Authorization</span></span>|<span data-ttu-id="3b8d7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b8d7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b8d7-125">Accept</span></span>|<span data-ttu-id="3b8d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b8d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b8d7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b8d7-127">Request body</span></span>
<span data-ttu-id="3b8d7-128">No corpo da solicitação, fornece uma representação JSON para o [objeto roleScopeTag.](../resources/intune-rbac-rolescopetag.md)</span><span class="sxs-lookup"><span data-stu-id="3b8d7-128">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="3b8d7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [a roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="3b8d7-129">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="3b8d7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b8d7-130">Property</span></span>|<span data-ttu-id="3b8d7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b8d7-131">Type</span></span>|<span data-ttu-id="3b8d7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b8d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b8d7-133">id</span><span class="sxs-lookup"><span data-stu-id="3b8d7-133">id</span></span>|<span data-ttu-id="3b8d7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b8d7-134">String</span></span>|<span data-ttu-id="3b8d7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-135">Key of the entity.</span></span> <span data-ttu-id="3b8d7-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="3b8d7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3b8d7-137">displayName</span></span>|<span data-ttu-id="3b8d7-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b8d7-138">String</span></span>|<span data-ttu-id="3b8d7-139">O nome de exibição ou amigável da Marca de Escopo de Função.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="3b8d7-140">descrição</span><span class="sxs-lookup"><span data-stu-id="3b8d7-140">description</span></span>|<span data-ttu-id="3b8d7-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b8d7-141">String</span></span>|<span data-ttu-id="3b8d7-142">Descrição da marca escopo de função.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-142">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="3b8d7-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="3b8d7-143">isBuiltIn</span></span>|<span data-ttu-id="3b8d7-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b8d7-144">Boolean</span></span>|<span data-ttu-id="3b8d7-145">Descrição da marca escopo de função.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-145">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="3b8d7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b8d7-146">Response</span></span>
<span data-ttu-id="3b8d7-147">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto roleScopeTag](../resources/intune-rbac-rolescopetag.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-147">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b8d7-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b8d7-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b8d7-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b8d7-149">Request</span></span>
<span data-ttu-id="3b8d7-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value",
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="3b8d7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b8d7-151">Response</span></span>
<span data-ttu-id="3b8d7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b8d7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




