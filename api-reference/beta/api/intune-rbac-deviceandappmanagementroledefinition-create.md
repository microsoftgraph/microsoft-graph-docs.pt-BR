---
title: Criar deviceAndAppManagementRoleDefinition
description: Cria um novo objeto deviceAndAppManagementRoleDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ba94c0169d751e6d4b1ade03fef7f7023847372
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801772"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="0ed53-103">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0ed53-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="0ed53-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ed53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ed53-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ed53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ed53-106">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0ed53-106">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ed53-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ed53-107">Prerequisites</span></span>
<span data-ttu-id="0ed53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ed53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ed53-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ed53-110">Permission type</span></span>|<span data-ttu-id="0ed53-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ed53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ed53-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ed53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ed53-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ed53-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0ed53-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ed53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ed53-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ed53-115">Not supported.</span></span>|
|<span data-ttu-id="0ed53-116">Application</span><span class="sxs-lookup"><span data-stu-id="0ed53-116">Application</span></span>|<span data-ttu-id="0ed53-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ed53-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ed53-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ed53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="0ed53-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ed53-119">Request headers</span></span>
|<span data-ttu-id="0ed53-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ed53-120">Header</span></span>|<span data-ttu-id="0ed53-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0ed53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ed53-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ed53-122">Authorization</span></span>|<span data-ttu-id="0ed53-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ed53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ed53-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ed53-124">Accept</span></span>|<span data-ttu-id="0ed53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ed53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ed53-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ed53-126">Request body</span></span>
<span data-ttu-id="0ed53-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="0ed53-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="0ed53-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="0ed53-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="0ed53-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ed53-129">Property</span></span>|<span data-ttu-id="0ed53-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ed53-130">Type</span></span>|<span data-ttu-id="0ed53-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ed53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ed53-132">id</span><span class="sxs-lookup"><span data-stu-id="0ed53-132">id</span></span>|<span data-ttu-id="0ed53-133">String</span><span class="sxs-lookup"><span data-stu-id="0ed53-133">String</span></span>|<span data-ttu-id="0ed53-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0ed53-134">Key of the entity.</span></span> <span data-ttu-id="0ed53-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0ed53-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="0ed53-136">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0ed53-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="0ed53-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0ed53-137">displayName</span></span>|<span data-ttu-id="0ed53-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ed53-138">String</span></span>|<span data-ttu-id="0ed53-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="0ed53-139">Display Name of the Role definition.</span></span> <span data-ttu-id="0ed53-140">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0ed53-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="0ed53-141">description</span><span class="sxs-lookup"><span data-stu-id="0ed53-141">description</span></span>|<span data-ttu-id="0ed53-142">String</span><span class="sxs-lookup"><span data-stu-id="0ed53-142">String</span></span>|<span data-ttu-id="0ed53-143">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="0ed53-143">Description of the Role definition.</span></span> <span data-ttu-id="0ed53-144">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0ed53-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="0ed53-145">permissões</span><span class="sxs-lookup"><span data-stu-id="0ed53-145">permissions</span></span>|<span data-ttu-id="0ed53-146">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="0ed53-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="0ed53-147">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="0ed53-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="0ed53-148">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="0ed53-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="0ed53-149">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0ed53-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="0ed53-150">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="0ed53-150">rolePermissions</span></span>|<span data-ttu-id="0ed53-151">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="0ed53-151">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="0ed53-152">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="0ed53-152">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="0ed53-153">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="0ed53-153">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="0ed53-154">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0ed53-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="0ed53-155">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0ed53-155">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="0ed53-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ed53-156">Boolean</span></span>|<span data-ttu-id="0ed53-157">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="0ed53-157">Type of Role.</span></span> <span data-ttu-id="0ed53-158">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="0ed53-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="0ed53-159">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0ed53-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="0ed53-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="0ed53-160">isBuiltIn</span></span>|<span data-ttu-id="0ed53-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ed53-161">Boolean</span></span>|<span data-ttu-id="0ed53-162">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="0ed53-162">Type of Role.</span></span> <span data-ttu-id="0ed53-163">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="0ed53-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="0ed53-164">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0ed53-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="0ed53-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ed53-165">roleScopeTagIds</span></span>|<span data-ttu-id="0ed53-166">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ed53-166">String collection</span></span>|<span data-ttu-id="0ed53-167">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0ed53-167">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ed53-168">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0ed53-168">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0ed53-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ed53-169">Response</span></span>
<span data-ttu-id="0ed53-170">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ed53-170">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ed53-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ed53-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ed53-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ed53-172">Request</span></span>
<span data-ttu-id="0ed53-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ed53-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="0ed53-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ed53-174">Response</span></span>
<span data-ttu-id="0ed53-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ed53-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




