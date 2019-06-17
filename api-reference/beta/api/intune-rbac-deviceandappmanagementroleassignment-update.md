---
title: Atualizar deviceAndAppManagementRoleAssignment
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 932c3a2ff17f072276610fb4ef29342261ededb6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988703"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="5dc36-103">Atualizar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5dc36-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="5dc36-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5dc36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dc36-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5dc36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dc36-106">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5dc36-106">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5dc36-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5dc36-107">Prerequisites</span></span>
<span data-ttu-id="5dc36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dc36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dc36-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dc36-110">Permission type</span></span>|<span data-ttu-id="5dc36-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5dc36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dc36-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dc36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5dc36-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dc36-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5dc36-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dc36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dc36-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc36-115">Not supported.</span></span>|
|<span data-ttu-id="5dc36-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dc36-116">Application</span></span>|<span data-ttu-id="5dc36-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dc36-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dc36-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dc36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5dc36-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc36-119">Request headers</span></span>
|<span data-ttu-id="5dc36-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5dc36-120">Header</span></span>|<span data-ttu-id="5dc36-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5dc36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dc36-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dc36-122">Authorization</span></span>|<span data-ttu-id="5dc36-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dc36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dc36-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5dc36-124">Accept</span></span>|<span data-ttu-id="5dc36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5dc36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dc36-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc36-126">Request body</span></span>
<span data-ttu-id="5dc36-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5dc36-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="5dc36-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5dc36-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="5dc36-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dc36-129">Property</span></span>|<span data-ttu-id="5dc36-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dc36-130">Type</span></span>|<span data-ttu-id="5dc36-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc36-132">id</span><span class="sxs-lookup"><span data-stu-id="5dc36-132">id</span></span>|<span data-ttu-id="5dc36-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc36-133">String</span></span>|<span data-ttu-id="5dc36-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5dc36-134">Key of the entity.</span></span> <span data-ttu-id="5dc36-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="5dc36-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="5dc36-136">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5dc36-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5dc36-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5dc36-137">displayName</span></span>|<span data-ttu-id="5dc36-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc36-138">String</span></span>|<span data-ttu-id="5dc36-139">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="5dc36-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="5dc36-140">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5dc36-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5dc36-141">descrição</span><span class="sxs-lookup"><span data-stu-id="5dc36-141">description</span></span>|<span data-ttu-id="5dc36-142">String</span><span class="sxs-lookup"><span data-stu-id="5dc36-142">String</span></span>|<span data-ttu-id="5dc36-143">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="5dc36-143">Description of the Role Assignment.</span></span> <span data-ttu-id="5dc36-144">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5dc36-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5dc36-145">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="5dc36-145">scopeMembers</span></span>|<span data-ttu-id="5dc36-146">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc36-146">String collection</span></span>|<span data-ttu-id="5dc36-147">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="5dc36-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="5dc36-148">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5dc36-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="5dc36-149">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5dc36-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5dc36-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="5dc36-150">scopeType</span></span>|[<span data-ttu-id="5dc36-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="5dc36-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="5dc36-152">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="5dc36-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="5dc36-153">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="5dc36-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="5dc36-154">Para ' mydevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="5dc36-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="5dc36-155">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5dc36-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="5dc36-156">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="5dc36-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="5dc36-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="5dc36-157">resourceScopes</span></span>|<span data-ttu-id="5dc36-158">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc36-158">String collection</span></span>|<span data-ttu-id="5dc36-159">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="5dc36-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="5dc36-160">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5dc36-160">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="5dc36-161">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5dc36-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="5dc36-162">members</span><span class="sxs-lookup"><span data-stu-id="5dc36-162">members</span></span>|<span data-ttu-id="5dc36-163">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc36-163">String collection</span></span>|<span data-ttu-id="5dc36-164">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="5dc36-164">The list of ids of role member security groups.</span></span> <span data-ttu-id="5dc36-165">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5dc36-165">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="5dc36-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc36-166">Response</span></span>
<span data-ttu-id="5dc36-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dc36-167">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dc36-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dc36-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="5dc36-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dc36-169">Request</span></span>
<span data-ttu-id="5dc36-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dc36-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5dc36-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dc36-171">Response</span></span>
<span data-ttu-id="5dc36-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dc36-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





