---
title: Atualizar deviceAndAppManagementRoleAssignment
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f4bc446f2a59244fcd6b02f157d25e260480524a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025673"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="06fe7-103">Atualizar deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="06fe7-103">Update deviceAndAppManagementRoleAssignment</span></span>

<span data-ttu-id="06fe7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06fe7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06fe7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06fe7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06fe7-106">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="06fe7-106">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06fe7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06fe7-107">Prerequisites</span></span>
<span data-ttu-id="06fe7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06fe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06fe7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06fe7-110">Permission type</span></span>|<span data-ttu-id="06fe7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06fe7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06fe7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06fe7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06fe7-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fe7-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="06fe7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06fe7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06fe7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06fe7-115">Not supported.</span></span>|
|<span data-ttu-id="06fe7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06fe7-116">Application</span></span>|<span data-ttu-id="06fe7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06fe7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06fe7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06fe7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="06fe7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06fe7-119">Request headers</span></span>
|<span data-ttu-id="06fe7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06fe7-120">Header</span></span>|<span data-ttu-id="06fe7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="06fe7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06fe7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="06fe7-122">Authorization</span></span>|<span data-ttu-id="06fe7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06fe7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06fe7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06fe7-124">Accept</span></span>|<span data-ttu-id="06fe7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06fe7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06fe7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06fe7-126">Request body</span></span>
<span data-ttu-id="06fe7-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="06fe7-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="06fe7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="06fe7-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="06fe7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06fe7-129">Property</span></span>|<span data-ttu-id="06fe7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="06fe7-130">Type</span></span>|<span data-ttu-id="06fe7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="06fe7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06fe7-132">id</span><span class="sxs-lookup"><span data-stu-id="06fe7-132">id</span></span>|<span data-ttu-id="06fe7-133">String</span><span class="sxs-lookup"><span data-stu-id="06fe7-133">String</span></span>|<span data-ttu-id="06fe7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06fe7-134">Key of the entity.</span></span> <span data-ttu-id="06fe7-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="06fe7-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="06fe7-136">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="06fe7-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="06fe7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="06fe7-137">displayName</span></span>|<span data-ttu-id="06fe7-138">String</span><span class="sxs-lookup"><span data-stu-id="06fe7-138">String</span></span>|<span data-ttu-id="06fe7-139">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="06fe7-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="06fe7-140">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="06fe7-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="06fe7-141">description</span><span class="sxs-lookup"><span data-stu-id="06fe7-141">description</span></span>|<span data-ttu-id="06fe7-142">String</span><span class="sxs-lookup"><span data-stu-id="06fe7-142">String</span></span>|<span data-ttu-id="06fe7-143">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="06fe7-143">Description of the Role Assignment.</span></span> <span data-ttu-id="06fe7-144">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="06fe7-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="06fe7-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="06fe7-145">resourceScopes</span></span>|<span data-ttu-id="06fe7-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="06fe7-146">String collection</span></span>|<span data-ttu-id="06fe7-147">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="06fe7-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="06fe7-148">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="06fe7-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="06fe7-149">Herdado de [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="06fe7-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="06fe7-150">members</span><span class="sxs-lookup"><span data-stu-id="06fe7-150">members</span></span>|<span data-ttu-id="06fe7-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="06fe7-151">String collection</span></span>|<span data-ttu-id="06fe7-152">A lista de IDs de grupos de segurança de membros da função.</span><span class="sxs-lookup"><span data-stu-id="06fe7-152">The list of ids of role member security groups.</span></span> <span data-ttu-id="06fe7-153">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="06fe7-153">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="06fe7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="06fe7-154">Response</span></span>
<span data-ttu-id="06fe7-155">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06fe7-155">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06fe7-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06fe7-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="06fe7-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06fe7-157">Request</span></span>
<span data-ttu-id="06fe7-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06fe7-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06fe7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="06fe7-159">Response</span></span>
<span data-ttu-id="06fe7-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06fe7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









