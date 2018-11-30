---
title: Atualizar deviceAndAppManagementRoleAssignment
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleAssignment.
ms.openlocfilehash: e5bf6040ce08a62ae557c8f137e0bd14c8b0b9a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006185"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="f03bc-103">Atualizar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f03bc-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="f03bc-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f03bc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f03bc-105">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f03bc-105">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f03bc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f03bc-106">Prerequisites</span></span>
<span data-ttu-id="f03bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f03bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f03bc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f03bc-109">Permission type</span></span>|<span data-ttu-id="f03bc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f03bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f03bc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f03bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f03bc-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f03bc-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f03bc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f03bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f03bc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f03bc-114">Not supported.</span></span>|
|<span data-ttu-id="f03bc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f03bc-115">Application</span></span>|<span data-ttu-id="f03bc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f03bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f03bc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f03bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f03bc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f03bc-118">Request headers</span></span>
|<span data-ttu-id="f03bc-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f03bc-119">Header</span></span>|<span data-ttu-id="f03bc-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f03bc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f03bc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f03bc-121">Authorization</span></span>|<span data-ttu-id="f03bc-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f03bc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f03bc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f03bc-123">Accept</span></span>|<span data-ttu-id="f03bc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f03bc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f03bc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f03bc-125">Request body</span></span>
<span data-ttu-id="f03bc-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f03bc-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="f03bc-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f03bc-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="f03bc-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f03bc-128">Property</span></span>|<span data-ttu-id="f03bc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f03bc-129">Type</span></span>|<span data-ttu-id="f03bc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f03bc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f03bc-131">id</span><span class="sxs-lookup"><span data-stu-id="f03bc-131">id</span></span>|<span data-ttu-id="f03bc-132">String</span><span class="sxs-lookup"><span data-stu-id="f03bc-132">String</span></span>|<span data-ttu-id="f03bc-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f03bc-133">Key of the entity.</span></span> <span data-ttu-id="f03bc-134">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="f03bc-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="f03bc-135">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f03bc-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f03bc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f03bc-136">displayName</span></span>|<span data-ttu-id="f03bc-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f03bc-137">String</span></span>|<span data-ttu-id="f03bc-138">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f03bc-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="f03bc-139">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f03bc-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f03bc-140">description</span><span class="sxs-lookup"><span data-stu-id="f03bc-140">description</span></span>|<span data-ttu-id="f03bc-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f03bc-141">String</span></span>|<span data-ttu-id="f03bc-142">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="f03bc-142">Description of the Role Assignment.</span></span> <span data-ttu-id="f03bc-143">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f03bc-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f03bc-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="f03bc-144">resourceScopes</span></span>|<span data-ttu-id="f03bc-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f03bc-145">String collection</span></span>|<span data-ttu-id="f03bc-146">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="f03bc-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="f03bc-147">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f03bc-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="f03bc-148">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f03bc-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f03bc-149">membros</span><span class="sxs-lookup"><span data-stu-id="f03bc-149">members</span></span>|<span data-ttu-id="f03bc-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f03bc-150">String collection</span></span>|<span data-ttu-id="f03bc-151">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="f03bc-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="f03bc-152">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f03bc-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="f03bc-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f03bc-153">Response</span></span>
<span data-ttu-id="f03bc-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f03bc-154">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f03bc-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f03bc-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="f03bc-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f03bc-156">Request</span></span>
<span data-ttu-id="f03bc-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f03bc-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="f03bc-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="f03bc-158">Response</span></span>
<span data-ttu-id="f03bc-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f03bc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



