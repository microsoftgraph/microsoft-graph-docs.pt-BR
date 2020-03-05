---
title: Atualizar deviceAndAppManagementRoleAssignment
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5939095b97fc7afd41ce2cf0cb150a7026fce4ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459832"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="02204-103">Atualizar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="02204-103">Update deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="02204-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="02204-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02204-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02204-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02204-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02204-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02204-107">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="02204-107">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02204-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02204-108">Prerequisites</span></span>
<span data-ttu-id="02204-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02204-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02204-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02204-111">Permission type</span></span>|<span data-ttu-id="02204-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02204-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02204-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02204-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02204-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02204-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="02204-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02204-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02204-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02204-116">Not supported.</span></span>|
|<span data-ttu-id="02204-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02204-117">Application</span></span>|<span data-ttu-id="02204-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02204-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02204-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02204-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="02204-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02204-120">Request headers</span></span>
|<span data-ttu-id="02204-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02204-121">Header</span></span>|<span data-ttu-id="02204-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02204-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02204-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02204-123">Authorization</span></span>|<span data-ttu-id="02204-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02204-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02204-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02204-125">Accept</span></span>|<span data-ttu-id="02204-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02204-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02204-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02204-127">Request body</span></span>
<span data-ttu-id="02204-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="02204-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="02204-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="02204-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="02204-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02204-130">Property</span></span>|<span data-ttu-id="02204-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02204-131">Type</span></span>|<span data-ttu-id="02204-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02204-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02204-133">id</span><span class="sxs-lookup"><span data-stu-id="02204-133">id</span></span>|<span data-ttu-id="02204-134">String</span><span class="sxs-lookup"><span data-stu-id="02204-134">String</span></span>|<span data-ttu-id="02204-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="02204-135">Key of the entity.</span></span> <span data-ttu-id="02204-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="02204-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="02204-137">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="02204-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="02204-138">displayName</span><span class="sxs-lookup"><span data-stu-id="02204-138">displayName</span></span>|<span data-ttu-id="02204-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02204-139">String</span></span>|<span data-ttu-id="02204-140">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="02204-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="02204-141">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="02204-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="02204-142">description</span><span class="sxs-lookup"><span data-stu-id="02204-142">description</span></span>|<span data-ttu-id="02204-143">String</span><span class="sxs-lookup"><span data-stu-id="02204-143">String</span></span>|<span data-ttu-id="02204-144">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="02204-144">Description of the Role Assignment.</span></span> <span data-ttu-id="02204-145">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="02204-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="02204-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="02204-146">scopeMembers</span></span>|<span data-ttu-id="02204-147">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02204-147">String collection</span></span>|<span data-ttu-id="02204-148">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="02204-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="02204-149">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="02204-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="02204-150">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="02204-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="02204-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="02204-151">scopeType</span></span>|[<span data-ttu-id="02204-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="02204-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="02204-153">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="02204-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="02204-154">O tipo padrão ' ResourceScope ' permite a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="02204-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="02204-155">Para ' mydevices ', ' AllLicensedUsers ' e ' AllDevicesAndLicensedUsers ', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="02204-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="02204-156">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="02204-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="02204-157">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="02204-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="02204-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="02204-158">resourceScopes</span></span>|<span data-ttu-id="02204-159">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02204-159">String collection</span></span>|<span data-ttu-id="02204-160">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="02204-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="02204-161">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="02204-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="02204-162">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="02204-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="02204-163">members</span><span class="sxs-lookup"><span data-stu-id="02204-163">members</span></span>|<span data-ttu-id="02204-164">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="02204-164">String collection</span></span>|<span data-ttu-id="02204-165">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="02204-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="02204-166">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="02204-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="02204-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="02204-167">Response</span></span>
<span data-ttu-id="02204-168">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02204-168">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02204-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02204-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="02204-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02204-170">Request</span></span>
<span data-ttu-id="02204-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02204-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="02204-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="02204-172">Response</span></span>
<span data-ttu-id="02204-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02204-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





