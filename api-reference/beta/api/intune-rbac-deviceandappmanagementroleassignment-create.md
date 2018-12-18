---
title: Criar deviceAndAppManagementRoleAssignment
description: Cria um novo objeto deviceAndAppManagementRoleAssignment.
author: tfitzmac
ms.openlocfilehash: 4ed81fdc58a2675be6d5f0b991507914d5c92e89
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323986"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="c5aaa-103">Criar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c5aaa-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="c5aaa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5aaa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5aaa-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5aaa-107">Cria um novo objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c5aaa-107">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5aaa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5aaa-108">Prerequisites</span></span>
<span data-ttu-id="c5aaa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5aaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5aaa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5aaa-111">Permission type</span></span>|<span data-ttu-id="c5aaa-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5aaa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5aaa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5aaa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5aaa-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5aaa-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c5aaa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5aaa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5aaa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-116">Not supported.</span></span>|
|<span data-ttu-id="c5aaa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5aaa-117">Application</span></span>|<span data-ttu-id="c5aaa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5aaa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5aaa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="c5aaa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5aaa-120">Request headers</span></span>
|<span data-ttu-id="c5aaa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5aaa-121">Header</span></span>|<span data-ttu-id="c5aaa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c5aaa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5aaa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5aaa-123">Authorization</span></span>|<span data-ttu-id="c5aaa-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5aaa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5aaa-125">Accept</span></span>|<span data-ttu-id="c5aaa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5aaa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5aaa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5aaa-127">Request body</span></span>
<span data-ttu-id="c5aaa-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="c5aaa-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="c5aaa-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5aaa-130">Property</span></span>|<span data-ttu-id="c5aaa-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5aaa-131">Type</span></span>|<span data-ttu-id="c5aaa-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5aaa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5aaa-133">id</span><span class="sxs-lookup"><span data-stu-id="c5aaa-133">id</span></span>|<span data-ttu-id="c5aaa-134">String</span><span class="sxs-lookup"><span data-stu-id="c5aaa-134">String</span></span>|<span data-ttu-id="c5aaa-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-135">Key of the entity.</span></span> <span data-ttu-id="c5aaa-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="c5aaa-137">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c5aaa-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="c5aaa-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c5aaa-138">displayName</span></span>|<span data-ttu-id="c5aaa-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5aaa-139">String</span></span>|<span data-ttu-id="c5aaa-140">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="c5aaa-141">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c5aaa-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="c5aaa-142">description</span><span class="sxs-lookup"><span data-stu-id="c5aaa-142">description</span></span>|<span data-ttu-id="c5aaa-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5aaa-143">String</span></span>|<span data-ttu-id="c5aaa-144">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-144">Description of the Role Assignment.</span></span> <span data-ttu-id="c5aaa-145">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c5aaa-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="c5aaa-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="c5aaa-146">scopeMembers</span></span>|<span data-ttu-id="c5aaa-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5aaa-147">String collection</span></span>|<span data-ttu-id="c5aaa-148">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="c5aaa-149">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="c5aaa-150">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c5aaa-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="c5aaa-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="c5aaa-151">scopeType</span></span>|[<span data-ttu-id="c5aaa-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="c5aaa-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="c5aaa-153">Especifica o tipo de escopo para uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="c5aaa-154">O tipo de padrão 'ResourceScope' permite que a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="c5aaa-155">Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="c5aaa-156">Herdada do [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c5aaa-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="c5aaa-157">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="c5aaa-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="c5aaa-158">resourceScopes</span></span>|<span data-ttu-id="c5aaa-159">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5aaa-159">String collection</span></span>|<span data-ttu-id="c5aaa-160">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="c5aaa-161">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="c5aaa-162">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c5aaa-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="c5aaa-163">membros</span><span class="sxs-lookup"><span data-stu-id="c5aaa-163">members</span></span>|<span data-ttu-id="c5aaa-164">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5aaa-164">String collection</span></span>|<span data-ttu-id="c5aaa-165">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="c5aaa-166">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="c5aaa-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5aaa-167">Response</span></span>
<span data-ttu-id="c5aaa-168">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-168">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5aaa-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5aaa-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5aaa-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5aaa-170">Request</span></span>
<span data-ttu-id="c5aaa-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5aaa-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5aaa-172">Response</span></span>
<span data-ttu-id="c5aaa-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5aaa-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





