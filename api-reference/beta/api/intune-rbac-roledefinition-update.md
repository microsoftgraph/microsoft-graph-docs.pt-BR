---
title: Atualizar roleDefinition
description: Atualizar as propriedades de um objeto roleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16163140c0e9f8548107590c88b8c0e6e2686b3b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899470"
---
# <a name="update-roledefinition"></a><span data-ttu-id="27738-103">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="27738-103">Update roleDefinition</span></span>

> <span data-ttu-id="27738-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27738-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27738-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27738-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27738-106">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="27738-106">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27738-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27738-107">Prerequisites</span></span>
<span data-ttu-id="27738-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27738-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27738-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27738-110">Permission type</span></span>|<span data-ttu-id="27738-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27738-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27738-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27738-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27738-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27738-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="27738-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27738-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27738-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27738-115">Not supported.</span></span>|
|<span data-ttu-id="27738-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27738-116">Application</span></span>|<span data-ttu-id="27738-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27738-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27738-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27738-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="27738-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27738-119">Request headers</span></span>
|<span data-ttu-id="27738-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27738-120">Header</span></span>|<span data-ttu-id="27738-121">Valor</span><span class="sxs-lookup"><span data-stu-id="27738-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27738-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27738-122">Authorization</span></span>|<span data-ttu-id="27738-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27738-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27738-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27738-124">Accept</span></span>|<span data-ttu-id="27738-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27738-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27738-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27738-126">Request body</span></span>
<span data-ttu-id="27738-127">No corpo da solicitação, forneça uma representação JSON do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="27738-127">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="27738-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="27738-128">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="27738-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27738-129">Property</span></span>|<span data-ttu-id="27738-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="27738-130">Type</span></span>|<span data-ttu-id="27738-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="27738-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27738-132">id</span><span class="sxs-lookup"><span data-stu-id="27738-132">id</span></span>|<span data-ttu-id="27738-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27738-133">String</span></span>|<span data-ttu-id="27738-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="27738-134">Key of the entity.</span></span> <span data-ttu-id="27738-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="27738-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="27738-136">displayName</span><span class="sxs-lookup"><span data-stu-id="27738-136">displayName</span></span>|<span data-ttu-id="27738-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27738-137">String</span></span>|<span data-ttu-id="27738-138">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="27738-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="27738-139">description</span><span class="sxs-lookup"><span data-stu-id="27738-139">description</span></span>|<span data-ttu-id="27738-140">String</span><span class="sxs-lookup"><span data-stu-id="27738-140">String</span></span>|<span data-ttu-id="27738-141">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="27738-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="27738-142">permissões</span><span class="sxs-lookup"><span data-stu-id="27738-142">permissions</span></span>|<span data-ttu-id="27738-143">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="27738-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="27738-144">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="27738-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="27738-145">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="27738-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="27738-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="27738-146">rolePermissions</span></span>|<span data-ttu-id="27738-147">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="27738-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="27738-148">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="27738-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="27738-149">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="27738-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="27738-150">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="27738-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="27738-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="27738-151">Boolean</span></span>|<span data-ttu-id="27738-152">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="27738-152">Type of Role.</span></span> <span data-ttu-id="27738-153">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="27738-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="27738-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="27738-154">isBuiltIn</span></span>|<span data-ttu-id="27738-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="27738-155">Boolean</span></span>|<span data-ttu-id="27738-156">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="27738-156">Type of Role.</span></span> <span data-ttu-id="27738-157">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="27738-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="27738-158">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="27738-158">roleScopeTagIds</span></span>|<span data-ttu-id="27738-159">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="27738-159">String collection</span></span>|<span data-ttu-id="27738-160">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="27738-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="27738-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="27738-161">Response</span></span>
<span data-ttu-id="27738-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27738-162">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27738-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27738-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="27738-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27738-164">Request</span></span>
<span data-ttu-id="27738-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27738-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="27738-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="27738-166">Response</span></span>
<span data-ttu-id="27738-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27738-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




