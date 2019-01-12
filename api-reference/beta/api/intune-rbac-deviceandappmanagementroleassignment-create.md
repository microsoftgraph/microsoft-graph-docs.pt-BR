---
title: Criar deviceAndAppManagementRoleAssignment
description: Cria um novo objeto deviceAndAppManagementRoleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 10e6a0a18fd41a26f3c29f4e10af76bdd1ccd1b5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984462"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="32bf6-103">Criar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="32bf6-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="32bf6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="32bf6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32bf6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="32bf6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32bf6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="32bf6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32bf6-107">Cria um novo objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32bf6-107">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32bf6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32bf6-108">Prerequisites</span></span>
<span data-ttu-id="32bf6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32bf6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32bf6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32bf6-111">Permission type</span></span>|<span data-ttu-id="32bf6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32bf6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32bf6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32bf6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32bf6-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32bf6-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="32bf6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32bf6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32bf6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32bf6-116">Not supported.</span></span>|
|<span data-ttu-id="32bf6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32bf6-117">Application</span></span>|<span data-ttu-id="32bf6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32bf6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32bf6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32bf6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="32bf6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32bf6-120">Request headers</span></span>
|<span data-ttu-id="32bf6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32bf6-121">Header</span></span>|<span data-ttu-id="32bf6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="32bf6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32bf6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="32bf6-123">Authorization</span></span>|<span data-ttu-id="32bf6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32bf6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32bf6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32bf6-125">Accept</span></span>|<span data-ttu-id="32bf6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32bf6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32bf6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32bf6-127">Request body</span></span>
<span data-ttu-id="32bf6-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="32bf6-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="32bf6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="32bf6-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="32bf6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32bf6-130">Property</span></span>|<span data-ttu-id="32bf6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="32bf6-131">Type</span></span>|<span data-ttu-id="32bf6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="32bf6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32bf6-133">id</span><span class="sxs-lookup"><span data-stu-id="32bf6-133">id</span></span>|<span data-ttu-id="32bf6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32bf6-134">String</span></span>|<span data-ttu-id="32bf6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="32bf6-135">Key of the entity.</span></span> <span data-ttu-id="32bf6-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="32bf6-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="32bf6-137">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="32bf6-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="32bf6-138">displayName</span><span class="sxs-lookup"><span data-stu-id="32bf6-138">displayName</span></span>|<span data-ttu-id="32bf6-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32bf6-139">String</span></span>|<span data-ttu-id="32bf6-140">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="32bf6-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="32bf6-141">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="32bf6-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="32bf6-142">description</span><span class="sxs-lookup"><span data-stu-id="32bf6-142">description</span></span>|<span data-ttu-id="32bf6-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32bf6-143">String</span></span>|<span data-ttu-id="32bf6-144">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="32bf6-144">Description of the Role Assignment.</span></span> <span data-ttu-id="32bf6-145">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="32bf6-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="32bf6-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="32bf6-146">scopeMembers</span></span>|<span data-ttu-id="32bf6-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="32bf6-147">String collection</span></span>|<span data-ttu-id="32bf6-148">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="32bf6-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="32bf6-149">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="32bf6-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="32bf6-150">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="32bf6-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="32bf6-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="32bf6-151">scopeType</span></span>|[<span data-ttu-id="32bf6-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="32bf6-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="32bf6-153">Especifica o tipo de escopo para uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="32bf6-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="32bf6-154">O tipo de padrão 'ResourceScope' permite que a atribuição de ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="32bf6-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="32bf6-155">Para 'AllDevices', 'AllLicensedUsers' e 'AllDevicesAndLicensedUsers', a propriedade ResourceScopes deve ser deixada vazia.</span><span class="sxs-lookup"><span data-stu-id="32bf6-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="32bf6-156">Herdada do [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32bf6-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="32bf6-157">Os valores possíveis são: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="32bf6-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="32bf6-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="32bf6-158">resourceScopes</span></span>|<span data-ttu-id="32bf6-159">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="32bf6-159">String collection</span></span>|<span data-ttu-id="32bf6-160">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="32bf6-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="32bf6-161">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="32bf6-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="32bf6-162">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="32bf6-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="32bf6-163">membros</span><span class="sxs-lookup"><span data-stu-id="32bf6-163">members</span></span>|<span data-ttu-id="32bf6-164">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="32bf6-164">String collection</span></span>|<span data-ttu-id="32bf6-165">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="32bf6-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="32bf6-166">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="32bf6-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="32bf6-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="32bf6-167">Response</span></span>
<span data-ttu-id="32bf6-168">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32bf6-168">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32bf6-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32bf6-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="32bf6-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32bf6-170">Request</span></span>
<span data-ttu-id="32bf6-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32bf6-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32bf6-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="32bf6-172">Response</span></span>
<span data-ttu-id="32bf6-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32bf6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





