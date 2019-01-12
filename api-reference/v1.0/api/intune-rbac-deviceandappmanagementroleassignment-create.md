---
title: Criar deviceAndAppManagementRoleAssignment
description: Cria um novo objeto deviceAndAppManagementRoleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 070db4890528c62443a66cedff3cf06723c5515e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985043"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="53b7c-103">Criar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="53b7c-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="53b7c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="53b7c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53b7c-105">Cria um novo objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="53b7c-105">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53b7c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53b7c-106">Prerequisites</span></span>
<span data-ttu-id="53b7c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53b7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b7c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53b7c-109">Permission type</span></span>|<span data-ttu-id="53b7c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53b7c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53b7c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53b7c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53b7c-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b7c-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="53b7c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53b7c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53b7c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53b7c-114">Not supported.</span></span>|
|<span data-ttu-id="53b7c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53b7c-115">Application</span></span>|<span data-ttu-id="53b7c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53b7c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53b7c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53b7c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="53b7c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53b7c-118">Request headers</span></span>
|<span data-ttu-id="53b7c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53b7c-119">Header</span></span>|<span data-ttu-id="53b7c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="53b7c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53b7c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="53b7c-121">Authorization</span></span>|<span data-ttu-id="53b7c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53b7c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53b7c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53b7c-123">Accept</span></span>|<span data-ttu-id="53b7c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53b7c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53b7c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53b7c-125">Request body</span></span>
<span data-ttu-id="53b7c-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="53b7c-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="53b7c-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceAndAppManagementRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="53b7c-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="53b7c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53b7c-128">Property</span></span>|<span data-ttu-id="53b7c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="53b7c-129">Type</span></span>|<span data-ttu-id="53b7c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="53b7c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b7c-131">id</span><span class="sxs-lookup"><span data-stu-id="53b7c-131">id</span></span>|<span data-ttu-id="53b7c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53b7c-132">String</span></span>|<span data-ttu-id="53b7c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="53b7c-133">Key of the entity.</span></span> <span data-ttu-id="53b7c-134">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="53b7c-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="53b7c-135">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="53b7c-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="53b7c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="53b7c-136">displayName</span></span>|<span data-ttu-id="53b7c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53b7c-137">String</span></span>|<span data-ttu-id="53b7c-138">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="53b7c-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="53b7c-139">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="53b7c-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="53b7c-140">description</span><span class="sxs-lookup"><span data-stu-id="53b7c-140">description</span></span>|<span data-ttu-id="53b7c-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53b7c-141">String</span></span>|<span data-ttu-id="53b7c-142">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="53b7c-142">Description of the Role Assignment.</span></span> <span data-ttu-id="53b7c-143">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="53b7c-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="53b7c-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="53b7c-144">resourceScopes</span></span>|<span data-ttu-id="53b7c-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="53b7c-145">String collection</span></span>|<span data-ttu-id="53b7c-146">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="53b7c-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="53b7c-147">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="53b7c-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="53b7c-148">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="53b7c-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="53b7c-149">membros</span><span class="sxs-lookup"><span data-stu-id="53b7c-149">members</span></span>|<span data-ttu-id="53b7c-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="53b7c-150">String collection</span></span>|<span data-ttu-id="53b7c-151">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="53b7c-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="53b7c-152">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="53b7c-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="53b7c-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="53b7c-153">Response</span></span>
<span data-ttu-id="53b7c-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53b7c-154">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53b7c-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53b7c-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="53b7c-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53b7c-156">Request</span></span>
<span data-ttu-id="53b7c-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53b7c-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
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

### <a name="response"></a><span data-ttu-id="53b7c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="53b7c-158">Response</span></span>
<span data-ttu-id="53b7c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53b7c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



