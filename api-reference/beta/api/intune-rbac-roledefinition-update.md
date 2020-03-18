---
title: Atualizar roleDefinition
description: Atualizar as propriedades de um objeto roleDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f4b92fb007f661e1307ad42db63976454bc2ebcb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801618"
---
# <a name="update-roledefinition"></a><span data-ttu-id="cf802-103">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="cf802-103">Update roleDefinition</span></span>

> <span data-ttu-id="cf802-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf802-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf802-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf802-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf802-106">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cf802-106">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf802-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf802-107">Prerequisites</span></span>
<span data-ttu-id="cf802-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf802-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf802-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf802-110">Permission type</span></span>|<span data-ttu-id="cf802-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf802-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf802-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf802-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf802-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf802-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="cf802-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf802-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf802-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf802-115">Not supported.</span></span>|
|<span data-ttu-id="cf802-116">Application</span><span class="sxs-lookup"><span data-stu-id="cf802-116">Application</span></span>|<span data-ttu-id="cf802-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf802-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf802-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf802-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="cf802-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf802-119">Request headers</span></span>
|<span data-ttu-id="cf802-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf802-120">Header</span></span>|<span data-ttu-id="cf802-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cf802-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf802-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf802-122">Authorization</span></span>|<span data-ttu-id="cf802-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf802-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf802-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf802-124">Accept</span></span>|<span data-ttu-id="cf802-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf802-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf802-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf802-126">Request body</span></span>
<span data-ttu-id="cf802-127">No corpo da solicitação, forneça uma representação JSON do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cf802-127">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="cf802-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cf802-128">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="cf802-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf802-129">Property</span></span>|<span data-ttu-id="cf802-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf802-130">Type</span></span>|<span data-ttu-id="cf802-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf802-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf802-132">id</span><span class="sxs-lookup"><span data-stu-id="cf802-132">id</span></span>|<span data-ttu-id="cf802-133">String</span><span class="sxs-lookup"><span data-stu-id="cf802-133">String</span></span>|<span data-ttu-id="cf802-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cf802-134">Key of the entity.</span></span> <span data-ttu-id="cf802-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="cf802-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="cf802-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cf802-136">displayName</span></span>|<span data-ttu-id="cf802-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf802-137">String</span></span>|<span data-ttu-id="cf802-138">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="cf802-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="cf802-139">description</span><span class="sxs-lookup"><span data-stu-id="cf802-139">description</span></span>|<span data-ttu-id="cf802-140">String</span><span class="sxs-lookup"><span data-stu-id="cf802-140">String</span></span>|<span data-ttu-id="cf802-141">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="cf802-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="cf802-142">permissões</span><span class="sxs-lookup"><span data-stu-id="cf802-142">permissions</span></span>|<span data-ttu-id="cf802-143">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="cf802-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="cf802-144">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="cf802-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="cf802-145">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="cf802-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="cf802-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="cf802-146">rolePermissions</span></span>|<span data-ttu-id="cf802-147">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="cf802-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="cf802-148">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="cf802-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="cf802-149">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="cf802-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="cf802-150">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cf802-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="cf802-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf802-151">Boolean</span></span>|<span data-ttu-id="cf802-152">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="cf802-152">Type of Role.</span></span> <span data-ttu-id="cf802-153">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="cf802-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="cf802-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="cf802-154">isBuiltIn</span></span>|<span data-ttu-id="cf802-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf802-155">Boolean</span></span>|<span data-ttu-id="cf802-156">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="cf802-156">Type of Role.</span></span> <span data-ttu-id="cf802-157">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="cf802-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="cf802-158">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cf802-158">roleScopeTagIds</span></span>|<span data-ttu-id="cf802-159">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf802-159">String collection</span></span>|<span data-ttu-id="cf802-160">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="cf802-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="cf802-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf802-161">Response</span></span>
<span data-ttu-id="cf802-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf802-162">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf802-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf802-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf802-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf802-164">Request</span></span>
<span data-ttu-id="cf802-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf802-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1207

{
  "@odata.type": "#microsoft.graph.roleDefinition",
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

### <a name="response"></a><span data-ttu-id="cf802-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf802-166">Response</span></span>
<span data-ttu-id="cf802-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf802-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1256

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
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




