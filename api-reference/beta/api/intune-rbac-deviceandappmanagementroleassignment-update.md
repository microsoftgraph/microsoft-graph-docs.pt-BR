---
title: Atualizar deviceAndAppManagementRoleAssignment
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20a1de5a901bb57f3bacf758de755ccb5177524e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43421329"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="1eeac-103">Atualizar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1eeac-103">Update deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="1eeac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1eeac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1eeac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1eeac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1eeac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1eeac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eeac-107">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1eeac-107">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1eeac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1eeac-108">Prerequisites</span></span>
<span data-ttu-id="1eeac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1eeac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1eeac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1eeac-111">Permission type</span></span>|<span data-ttu-id="1eeac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1eeac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1eeac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1eeac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1eeac-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eeac-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="1eeac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1eeac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1eeac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1eeac-116">Not supported.</span></span>|
|<span data-ttu-id="1eeac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1eeac-117">Application</span></span>|<span data-ttu-id="1eeac-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eeac-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1eeac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1eeac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1eeac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1eeac-120">Request headers</span></span>
|<span data-ttu-id="1eeac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1eeac-121">Header</span></span>|<span data-ttu-id="1eeac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1eeac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1eeac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1eeac-123">Authorization</span></span>|<span data-ttu-id="1eeac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1eeac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1eeac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1eeac-125">Accept</span></span>|<span data-ttu-id="1eeac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1eeac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1eeac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1eeac-127">Request body</span></span>
<span data-ttu-id="1eeac-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1eeac-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="1eeac-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1eeac-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="1eeac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1eeac-130">Property</span></span>|<span data-ttu-id="1eeac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1eeac-131">Type</span></span>|<span data-ttu-id="1eeac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1eeac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eeac-133">id</span><span class="sxs-lookup"><span data-stu-id="1eeac-133">id</span></span>|<span data-ttu-id="1eeac-134">String</span><span class="sxs-lookup"><span data-stu-id="1eeac-134">String</span></span>|<span data-ttu-id="1eeac-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1eeac-135">Key of the entity.</span></span> <span data-ttu-id="1eeac-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="1eeac-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="1eeac-137">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1eeac-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="1eeac-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1eeac-138">displayName</span></span>|<span data-ttu-id="1eeac-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1eeac-139">String</span></span>|<span data-ttu-id="1eeac-140">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="1eeac-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="1eeac-141">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1eeac-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="1eeac-142">description</span><span class="sxs-lookup"><span data-stu-id="1eeac-142">description</span></span>|<span data-ttu-id="1eeac-143">String</span><span class="sxs-lookup"><span data-stu-id="1eeac-143">String</span></span>|<span data-ttu-id="1eeac-144">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="1eeac-144">Description of the Role Assignment.</span></span> <span data-ttu-id="1eeac-145">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1eeac-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="1eeac-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="1eeac-146">scopeMembers</span></span>|<span data-ttu-id="1eeac-147">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1eeac-147">String collection</span></span>|<span data-ttu-id="1eeac-148">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="1eeac-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="1eeac-149">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1eeac-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="1eeac-150">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1eeac-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="1eeac-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="1eeac-151">scopeType</span></span>|[<span data-ttu-id="1eeac-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="1eeac-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="1eeac-153">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="1eeac-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="1eeac-154">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="1eeac-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="1eeac-155">Para ' mydevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="1eeac-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="1eeac-156">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1eeac-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="1eeac-157">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="1eeac-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="1eeac-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="1eeac-158">resourceScopes</span></span>|<span data-ttu-id="1eeac-159">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1eeac-159">String collection</span></span>|<span data-ttu-id="1eeac-160">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="1eeac-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="1eeac-161">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1eeac-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="1eeac-162">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1eeac-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="1eeac-163">members</span><span class="sxs-lookup"><span data-stu-id="1eeac-163">members</span></span>|<span data-ttu-id="1eeac-164">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1eeac-164">String collection</span></span>|<span data-ttu-id="1eeac-165">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="1eeac-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="1eeac-166">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1eeac-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="1eeac-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eeac-167">Response</span></span>
<span data-ttu-id="1eeac-168">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1eeac-168">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1eeac-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1eeac-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="1eeac-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1eeac-170">Request</span></span>
<span data-ttu-id="1eeac-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1eeac-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="1eeac-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eeac-172">Response</span></span>
<span data-ttu-id="1eeac-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1eeac-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



