---
title: Atualizar deviceAndAppManagementRoleDefinition
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4061ef29268343adbb623cf9c7fe018bdce60517
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43421293"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="d54b8-103">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d54b8-103">Update deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="d54b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d54b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d54b8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d54b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d54b8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d54b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d54b8-107">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d54b8-107">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d54b8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d54b8-108">Prerequisites</span></span>
<span data-ttu-id="d54b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d54b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d54b8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d54b8-111">Permission type</span></span>|<span data-ttu-id="d54b8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d54b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d54b8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d54b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d54b8-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d54b8-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d54b8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d54b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d54b8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d54b8-116">Not supported.</span></span>|
|<span data-ttu-id="d54b8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d54b8-117">Application</span></span>|<span data-ttu-id="d54b8-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d54b8-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d54b8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d54b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="d54b8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d54b8-120">Request headers</span></span>
|<span data-ttu-id="d54b8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d54b8-121">Header</span></span>|<span data-ttu-id="d54b8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d54b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d54b8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d54b8-123">Authorization</span></span>|<span data-ttu-id="d54b8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d54b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d54b8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d54b8-125">Accept</span></span>|<span data-ttu-id="d54b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d54b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d54b8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d54b8-127">Request body</span></span>
<span data-ttu-id="d54b8-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d54b8-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="d54b8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d54b8-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="d54b8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d54b8-130">Property</span></span>|<span data-ttu-id="d54b8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d54b8-131">Type</span></span>|<span data-ttu-id="d54b8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d54b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d54b8-133">id</span><span class="sxs-lookup"><span data-stu-id="d54b8-133">id</span></span>|<span data-ttu-id="d54b8-134">String</span><span class="sxs-lookup"><span data-stu-id="d54b8-134">String</span></span>|<span data-ttu-id="d54b8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d54b8-135">Key of the entity.</span></span> <span data-ttu-id="d54b8-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d54b8-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="d54b8-137">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d54b8-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d54b8-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d54b8-138">displayName</span></span>|<span data-ttu-id="d54b8-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d54b8-139">String</span></span>|<span data-ttu-id="d54b8-140">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="d54b8-140">Display Name of the Role definition.</span></span> <span data-ttu-id="d54b8-141">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d54b8-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d54b8-142">description</span><span class="sxs-lookup"><span data-stu-id="d54b8-142">description</span></span>|<span data-ttu-id="d54b8-143">String</span><span class="sxs-lookup"><span data-stu-id="d54b8-143">String</span></span>|<span data-ttu-id="d54b8-144">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="d54b8-144">Description of the Role definition.</span></span> <span data-ttu-id="d54b8-145">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d54b8-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d54b8-146">permissões</span><span class="sxs-lookup"><span data-stu-id="d54b8-146">permissions</span></span>|<span data-ttu-id="d54b8-147">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="d54b8-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="d54b8-148">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="d54b8-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="d54b8-149">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="d54b8-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="d54b8-150">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d54b8-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d54b8-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="d54b8-151">rolePermissions</span></span>|<span data-ttu-id="d54b8-152">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="d54b8-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="d54b8-153">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="d54b8-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="d54b8-154">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="d54b8-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="d54b8-155">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d54b8-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d54b8-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d54b8-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="d54b8-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="d54b8-157">Boolean</span></span>|<span data-ttu-id="d54b8-158">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="d54b8-158">Type of Role.</span></span> <span data-ttu-id="d54b8-159">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="d54b8-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="d54b8-160">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d54b8-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d54b8-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="d54b8-161">isBuiltIn</span></span>|<span data-ttu-id="d54b8-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="d54b8-162">Boolean</span></span>|<span data-ttu-id="d54b8-163">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="d54b8-163">Type of Role.</span></span> <span data-ttu-id="d54b8-164">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="d54b8-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="d54b8-165">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d54b8-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d54b8-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d54b8-166">roleScopeTagIds</span></span>|<span data-ttu-id="d54b8-167">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d54b8-167">String collection</span></span>|<span data-ttu-id="d54b8-168">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d54b8-168">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d54b8-169">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d54b8-169">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d54b8-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="d54b8-170">Response</span></span>
<span data-ttu-id="d54b8-171">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d54b8-171">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d54b8-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d54b8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="d54b8-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d54b8-173">Request</span></span>
<span data-ttu-id="d54b8-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d54b8-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1229

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
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
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
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
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d54b8-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="d54b8-175">Response</span></span>
<span data-ttu-id="d54b8-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d54b8-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1278

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
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
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
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
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```



