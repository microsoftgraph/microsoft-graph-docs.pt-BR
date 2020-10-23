---
title: Criar deviceAndAppManagementRoleDefinition
description: Cria um novo objeto deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4baf3947795cf35236f5c52cb4b6c2c36b49262c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725972"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="475f4-103">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="475f4-103">Create deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="475f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="475f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="475f4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="475f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="475f4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="475f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="475f4-107">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="475f4-107">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="475f4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="475f4-108">Prerequisites</span></span>
<span data-ttu-id="475f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="475f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="475f4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="475f4-111">Permission type</span></span>|<span data-ttu-id="475f4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="475f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="475f4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="475f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="475f4-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="475f4-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="475f4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="475f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="475f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="475f4-116">Not supported.</span></span>|
|<span data-ttu-id="475f4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="475f4-117">Application</span></span>|<span data-ttu-id="475f4-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="475f4-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="475f4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="475f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="475f4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="475f4-120">Request headers</span></span>
|<span data-ttu-id="475f4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="475f4-121">Header</span></span>|<span data-ttu-id="475f4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="475f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="475f4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="475f4-123">Authorization</span></span>|<span data-ttu-id="475f4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="475f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="475f4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="475f4-125">Accept</span></span>|<span data-ttu-id="475f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="475f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="475f4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="475f4-127">Request body</span></span>
<span data-ttu-id="475f4-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="475f4-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="475f4-129">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="475f4-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="475f4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="475f4-130">Property</span></span>|<span data-ttu-id="475f4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="475f4-131">Type</span></span>|<span data-ttu-id="475f4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="475f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="475f4-133">id</span><span class="sxs-lookup"><span data-stu-id="475f4-133">id</span></span>|<span data-ttu-id="475f4-134">String</span><span class="sxs-lookup"><span data-stu-id="475f4-134">String</span></span>|<span data-ttu-id="475f4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="475f4-135">Key of the entity.</span></span> <span data-ttu-id="475f4-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="475f4-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="475f4-137">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="475f4-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="475f4-138">displayName</span><span class="sxs-lookup"><span data-stu-id="475f4-138">displayName</span></span>|<span data-ttu-id="475f4-139">String</span><span class="sxs-lookup"><span data-stu-id="475f4-139">String</span></span>|<span data-ttu-id="475f4-140">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="475f4-140">Display Name of the Role definition.</span></span> <span data-ttu-id="475f4-141">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="475f4-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="475f4-142">description</span><span class="sxs-lookup"><span data-stu-id="475f4-142">description</span></span>|<span data-ttu-id="475f4-143">String</span><span class="sxs-lookup"><span data-stu-id="475f4-143">String</span></span>|<span data-ttu-id="475f4-144">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="475f4-144">Description of the Role definition.</span></span> <span data-ttu-id="475f4-145">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="475f4-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="475f4-146">permissões</span><span class="sxs-lookup"><span data-stu-id="475f4-146">permissions</span></span>|<span data-ttu-id="475f4-147">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="475f4-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="475f4-148">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="475f4-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="475f4-149">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="475f4-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="475f4-150">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="475f4-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="475f4-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="475f4-151">rolePermissions</span></span>|<span data-ttu-id="475f4-152">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="475f4-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="475f4-153">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="475f4-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="475f4-154">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="475f4-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="475f4-155">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="475f4-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="475f4-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="475f4-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="475f4-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="475f4-157">Boolean</span></span>|<span data-ttu-id="475f4-158">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="475f4-158">Type of Role.</span></span> <span data-ttu-id="475f4-159">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="475f4-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="475f4-160">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="475f4-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="475f4-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="475f4-161">isBuiltIn</span></span>|<span data-ttu-id="475f4-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="475f4-162">Boolean</span></span>|<span data-ttu-id="475f4-163">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="475f4-163">Type of Role.</span></span> <span data-ttu-id="475f4-164">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="475f4-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="475f4-165">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="475f4-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="475f4-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="475f4-166">roleScopeTagIds</span></span>|<span data-ttu-id="475f4-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="475f4-167">String collection</span></span>|<span data-ttu-id="475f4-168">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="475f4-168">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="475f4-169">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="475f4-169">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="475f4-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="475f4-170">Response</span></span>
<span data-ttu-id="475f4-171">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="475f4-171">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="475f4-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="475f4-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="475f4-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="475f4-173">Request</span></span>
<span data-ttu-id="475f4-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="475f4-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="475f4-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="475f4-175">Response</span></span>
<span data-ttu-id="475f4-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="475f4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





