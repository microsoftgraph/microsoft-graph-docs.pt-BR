---
title: Criar deviceAndAppManagementRoleAssignment
description: Cria um novo objeto deviceAndAppManagementRoleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4df222bc2049fd7034e062eb2e6af8a86684cde6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778513"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="34975-103">Criar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="34975-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="34975-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34975-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34975-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34975-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34975-106">Cria um novo objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="34975-106">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34975-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34975-107">Prerequisites</span></span>
<span data-ttu-id="34975-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34975-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34975-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34975-110">Permission type</span></span>|<span data-ttu-id="34975-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34975-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34975-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34975-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34975-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34975-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="34975-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34975-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34975-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34975-115">Not supported.</span></span>|
|<span data-ttu-id="34975-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34975-116">Application</span></span>|<span data-ttu-id="34975-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34975-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34975-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34975-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="34975-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34975-119">Request headers</span></span>
|<span data-ttu-id="34975-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34975-120">Header</span></span>|<span data-ttu-id="34975-121">Valor</span><span class="sxs-lookup"><span data-stu-id="34975-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34975-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34975-122">Authorization</span></span>|<span data-ttu-id="34975-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34975-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34975-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34975-124">Accept</span></span>|<span data-ttu-id="34975-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34975-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34975-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34975-126">Request body</span></span>
<span data-ttu-id="34975-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="34975-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="34975-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="34975-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="34975-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34975-129">Property</span></span>|<span data-ttu-id="34975-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="34975-130">Type</span></span>|<span data-ttu-id="34975-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="34975-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34975-132">id</span><span class="sxs-lookup"><span data-stu-id="34975-132">id</span></span>|<span data-ttu-id="34975-133">String</span><span class="sxs-lookup"><span data-stu-id="34975-133">String</span></span>|<span data-ttu-id="34975-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="34975-134">Key of the entity.</span></span> <span data-ttu-id="34975-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="34975-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="34975-136">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="34975-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="34975-137">displayName</span><span class="sxs-lookup"><span data-stu-id="34975-137">displayName</span></span>|<span data-ttu-id="34975-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34975-138">String</span></span>|<span data-ttu-id="34975-139">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="34975-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="34975-140">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="34975-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="34975-141">description</span><span class="sxs-lookup"><span data-stu-id="34975-141">description</span></span>|<span data-ttu-id="34975-142">String</span><span class="sxs-lookup"><span data-stu-id="34975-142">String</span></span>|<span data-ttu-id="34975-143">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="34975-143">Description of the Role Assignment.</span></span> <span data-ttu-id="34975-144">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="34975-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="34975-145">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="34975-145">scopeMembers</span></span>|<span data-ttu-id="34975-146">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34975-146">String collection</span></span>|<span data-ttu-id="34975-147">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="34975-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="34975-148">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="34975-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="34975-149">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="34975-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="34975-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="34975-150">scopeType</span></span>|[<span data-ttu-id="34975-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="34975-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="34975-152">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="34975-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="34975-153">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="34975-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="34975-154">Para ' myDevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="34975-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="34975-155">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="34975-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="34975-156">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="34975-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="34975-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="34975-157">resourceScopes</span></span>|<span data-ttu-id="34975-158">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34975-158">String collection</span></span>|<span data-ttu-id="34975-159">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="34975-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="34975-160">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="34975-160">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="34975-161">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="34975-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="34975-162">members</span><span class="sxs-lookup"><span data-stu-id="34975-162">members</span></span>|<span data-ttu-id="34975-163">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="34975-163">String collection</span></span>|<span data-ttu-id="34975-164">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="34975-164">The list of ids of role member security groups.</span></span> <span data-ttu-id="34975-165">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="34975-165">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="34975-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="34975-166">Response</span></span>
<span data-ttu-id="34975-167">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34975-167">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34975-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34975-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="34975-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34975-169">Request</span></span>
<span data-ttu-id="34975-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34975-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleAssignments
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

### <a name="response"></a><span data-ttu-id="34975-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="34975-171">Response</span></span>
<span data-ttu-id="34975-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34975-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





