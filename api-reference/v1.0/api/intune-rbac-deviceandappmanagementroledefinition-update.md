---
title: Atualizar deviceAndAppManagementRoleDefinition
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 05388f7a6aa54d279a6de9e3ce5ecce929474d25
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43452629"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="ffaba-103">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ffaba-103">Update deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="ffaba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffaba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffaba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ffaba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffaba-106">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ffaba-106">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffaba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ffaba-107">Prerequisites</span></span>
<span data-ttu-id="ffaba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffaba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffaba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ffaba-110">Permission type</span></span>|<span data-ttu-id="ffaba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ffaba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffaba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ffaba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ffaba-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffaba-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ffaba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ffaba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffaba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffaba-115">Not supported.</span></span>|
|<span data-ttu-id="ffaba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ffaba-116">Application</span></span>|<span data-ttu-id="ffaba-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffaba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffaba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ffaba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="ffaba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ffaba-119">Request headers</span></span>
|<span data-ttu-id="ffaba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ffaba-120">Header</span></span>|<span data-ttu-id="ffaba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ffaba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffaba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ffaba-122">Authorization</span></span>|<span data-ttu-id="ffaba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ffaba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffaba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ffaba-124">Accept</span></span>|<span data-ttu-id="ffaba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ffaba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffaba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ffaba-126">Request body</span></span>
<span data-ttu-id="ffaba-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ffaba-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="ffaba-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ffaba-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="ffaba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffaba-129">Property</span></span>|<span data-ttu-id="ffaba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffaba-130">Type</span></span>|<span data-ttu-id="ffaba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffaba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffaba-132">id</span><span class="sxs-lookup"><span data-stu-id="ffaba-132">id</span></span>|<span data-ttu-id="ffaba-133">String</span><span class="sxs-lookup"><span data-stu-id="ffaba-133">String</span></span>|<span data-ttu-id="ffaba-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ffaba-134">Key of the entity.</span></span> <span data-ttu-id="ffaba-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="ffaba-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="ffaba-136">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ffaba-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ffaba-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ffaba-137">displayName</span></span>|<span data-ttu-id="ffaba-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ffaba-138">String</span></span>|<span data-ttu-id="ffaba-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="ffaba-139">Display Name of the Role definition.</span></span> <span data-ttu-id="ffaba-140">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ffaba-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ffaba-141">description</span><span class="sxs-lookup"><span data-stu-id="ffaba-141">description</span></span>|<span data-ttu-id="ffaba-142">String</span><span class="sxs-lookup"><span data-stu-id="ffaba-142">String</span></span>|<span data-ttu-id="ffaba-143">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="ffaba-143">Description of the Role definition.</span></span> <span data-ttu-id="ffaba-144">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ffaba-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ffaba-145">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ffaba-145">rolePermissions</span></span>|<span data-ttu-id="ffaba-146">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ffaba-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ffaba-147">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="ffaba-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ffaba-148">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="ffaba-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ffaba-149">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ffaba-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ffaba-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ffaba-150">isBuiltIn</span></span>|<span data-ttu-id="ffaba-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffaba-151">Boolean</span></span>|<span data-ttu-id="ffaba-152">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="ffaba-152">Type of Role.</span></span> <span data-ttu-id="ffaba-153">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="ffaba-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ffaba-154">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ffaba-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ffaba-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffaba-155">Response</span></span>
<span data-ttu-id="ffaba-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ffaba-156">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffaba-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ffaba-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffaba-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ffaba-158">Request</span></span>
<span data-ttu-id="ffaba-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ffaba-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="ffaba-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffaba-160">Response</span></span>
<span data-ttu-id="ffaba-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ffaba-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```






