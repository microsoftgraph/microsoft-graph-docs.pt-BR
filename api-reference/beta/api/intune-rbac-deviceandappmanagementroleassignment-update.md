---
title: Atualizar deviceAndAppManagementRoleAssignment
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1cbdc5b74b0143189872f9117e619a827741d7eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416493"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="044c3-103">Atualizar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="044c3-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="044c3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="044c3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="044c3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="044c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="044c3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="044c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="044c3-107">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="044c3-107">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="044c3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="044c3-108">Prerequisites</span></span>
<span data-ttu-id="044c3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="044c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="044c3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="044c3-111">Permission type</span></span>|<span data-ttu-id="044c3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="044c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="044c3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="044c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="044c3-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="044c3-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="044c3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="044c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="044c3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="044c3-116">Not supported.</span></span>|
|<span data-ttu-id="044c3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="044c3-117">Application</span></span>|<span data-ttu-id="044c3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="044c3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="044c3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="044c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="044c3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="044c3-120">Request headers</span></span>
|<span data-ttu-id="044c3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="044c3-121">Header</span></span>|<span data-ttu-id="044c3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="044c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="044c3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="044c3-123">Authorization</span></span>|<span data-ttu-id="044c3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="044c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="044c3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="044c3-125">Accept</span></span>|<span data-ttu-id="044c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="044c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="044c3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="044c3-127">Request body</span></span>
<span data-ttu-id="044c3-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="044c3-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="044c3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="044c3-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="044c3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="044c3-130">Property</span></span>|<span data-ttu-id="044c3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="044c3-131">Type</span></span>|<span data-ttu-id="044c3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="044c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="044c3-133">id</span><span class="sxs-lookup"><span data-stu-id="044c3-133">id</span></span>|<span data-ttu-id="044c3-134">String</span><span class="sxs-lookup"><span data-stu-id="044c3-134">String</span></span>|<span data-ttu-id="044c3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="044c3-135">Key of the entity.</span></span> <span data-ttu-id="044c3-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="044c3-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="044c3-137">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="044c3-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="044c3-138">displayName</span><span class="sxs-lookup"><span data-stu-id="044c3-138">displayName</span></span>|<span data-ttu-id="044c3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="044c3-139">String</span></span>|<span data-ttu-id="044c3-140">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="044c3-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="044c3-141">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="044c3-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="044c3-142">description</span><span class="sxs-lookup"><span data-stu-id="044c3-142">description</span></span>|<span data-ttu-id="044c3-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="044c3-143">String</span></span>|<span data-ttu-id="044c3-144">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="044c3-144">Description of the Role Assignment.</span></span> <span data-ttu-id="044c3-145">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="044c3-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="044c3-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="044c3-146">scopeMembers</span></span>|<span data-ttu-id="044c3-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="044c3-147">String collection</span></span>|<span data-ttu-id="044c3-148">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="044c3-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="044c3-149">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="044c3-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="044c3-150">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="044c3-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="044c3-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="044c3-151">scopeType</span></span>|[<span data-ttu-id="044c3-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="044c3-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="044c3-153">Especifica o tipo de escopo para uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="044c3-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="044c3-154">O tipo de padrão 'ResourceScope' permite que a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="044c3-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="044c3-155">Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="044c3-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="044c3-156">Herdada do [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="044c3-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="044c3-157">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="044c3-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="044c3-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="044c3-158">resourceScopes</span></span>|<span data-ttu-id="044c3-159">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="044c3-159">String collection</span></span>|<span data-ttu-id="044c3-160">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="044c3-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="044c3-161">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="044c3-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="044c3-162">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="044c3-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="044c3-163">membros</span><span class="sxs-lookup"><span data-stu-id="044c3-163">members</span></span>|<span data-ttu-id="044c3-164">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="044c3-164">String collection</span></span>|<span data-ttu-id="044c3-165">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="044c3-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="044c3-166">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="044c3-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="044c3-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="044c3-167">Response</span></span>
<span data-ttu-id="044c3-168">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="044c3-168">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="044c3-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="044c3-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="044c3-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="044c3-170">Request</span></span>
<span data-ttu-id="044c3-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="044c3-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="044c3-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="044c3-172">Response</span></span>
<span data-ttu-id="044c3-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="044c3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




