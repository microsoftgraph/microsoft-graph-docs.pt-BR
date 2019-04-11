---
title: Criar roleDefinition
description: Criar um novo objeto roleDefinition
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3949cf3dbeab5a9c6c1717d2103c574f532aad46
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772927"
---
# <a name="create-roledefinition"></a><span data-ttu-id="3a36f-103">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3a36f-103">Create roleDefinition</span></span>

> <span data-ttu-id="3a36f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a36f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a36f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a36f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a36f-106">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3a36f-106">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a36f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a36f-107">Prerequisites</span></span>
<span data-ttu-id="3a36f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a36f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a36f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a36f-110">Permission type</span></span>|<span data-ttu-id="3a36f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3a36f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a36f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a36f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3a36f-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a36f-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3a36f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a36f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a36f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a36f-115">Not supported.</span></span>|
|<span data-ttu-id="3a36f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a36f-116">Application</span></span>|<span data-ttu-id="3a36f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a36f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a36f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a36f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="3a36f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a36f-119">Request headers</span></span>
|<span data-ttu-id="3a36f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a36f-120">Header</span></span>|<span data-ttu-id="3a36f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3a36f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a36f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a36f-122">Authorization</span></span>|<span data-ttu-id="3a36f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a36f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a36f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3a36f-124">Accept</span></span>|<span data-ttu-id="3a36f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3a36f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a36f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a36f-126">Request body</span></span>
<span data-ttu-id="3a36f-127">No corpo da solicitação, forneça uma representação JSON do objeto roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="3a36f-127">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="3a36f-128">A tabela a seguir mostra as propriedades obrigatórias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="3a36f-128">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="3a36f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a36f-129">Property</span></span>|<span data-ttu-id="3a36f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a36f-130">Type</span></span>|<span data-ttu-id="3a36f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a36f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a36f-132">id</span><span class="sxs-lookup"><span data-stu-id="3a36f-132">id</span></span>|<span data-ttu-id="3a36f-133">String</span><span class="sxs-lookup"><span data-stu-id="3a36f-133">String</span></span>|<span data-ttu-id="3a36f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3a36f-134">Key of the entity.</span></span> <span data-ttu-id="3a36f-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3a36f-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="3a36f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3a36f-136">displayName</span></span>|<span data-ttu-id="3a36f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a36f-137">String</span></span>|<span data-ttu-id="3a36f-138">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="3a36f-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="3a36f-139">description</span><span class="sxs-lookup"><span data-stu-id="3a36f-139">description</span></span>|<span data-ttu-id="3a36f-140">String</span><span class="sxs-lookup"><span data-stu-id="3a36f-140">String</span></span>|<span data-ttu-id="3a36f-141">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="3a36f-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="3a36f-142">permissões</span><span class="sxs-lookup"><span data-stu-id="3a36f-142">permissions</span></span>|<span data-ttu-id="3a36f-143">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3a36f-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3a36f-144">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="3a36f-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3a36f-145">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3a36f-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="3a36f-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="3a36f-146">rolePermissions</span></span>|<span data-ttu-id="3a36f-147">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3a36f-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3a36f-148">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="3a36f-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3a36f-149">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3a36f-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="3a36f-150">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3a36f-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="3a36f-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="3a36f-151">Boolean</span></span>|<span data-ttu-id="3a36f-152">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="3a36f-152">Type of Role.</span></span> <span data-ttu-id="3a36f-153">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="3a36f-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="3a36f-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="3a36f-154">isBuiltIn</span></span>|<span data-ttu-id="3a36f-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="3a36f-155">Boolean</span></span>|<span data-ttu-id="3a36f-156">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="3a36f-156">Type of Role.</span></span> <span data-ttu-id="3a36f-157">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="3a36f-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="3a36f-158">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a36f-158">roleScopeTagIds</span></span>|<span data-ttu-id="3a36f-159">Coleção String</span><span class="sxs-lookup"><span data-stu-id="3a36f-159">String collection</span></span>|<span data-ttu-id="3a36f-160">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3a36f-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="3a36f-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a36f-161">Response</span></span>
<span data-ttu-id="3a36f-162">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a36f-162">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a36f-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a36f-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a36f-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a36f-164">Request</span></span>
<span data-ttu-id="3a36f-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a36f-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="3a36f-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a36f-166">Response</span></span>
<span data-ttu-id="3a36f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a36f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





