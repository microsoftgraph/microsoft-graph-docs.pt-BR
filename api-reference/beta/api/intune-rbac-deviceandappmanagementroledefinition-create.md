---
title: Criar deviceAndAppManagementRoleDefinition
description: Cria um novo objeto deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9017d2cd02fa7ef9594efb62b168ce70fc4dd259
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139575"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="aac69-103">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="aac69-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="aac69-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aac69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aac69-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aac69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aac69-106">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="aac69-106">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aac69-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aac69-107">Prerequisites</span></span>
<span data-ttu-id="aac69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aac69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aac69-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aac69-110">Permission type</span></span>|<span data-ttu-id="aac69-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aac69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aac69-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aac69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aac69-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac69-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="aac69-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aac69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aac69-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aac69-115">Not supported.</span></span>|
|<span data-ttu-id="aac69-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aac69-116">Application</span></span>|<span data-ttu-id="aac69-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aac69-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aac69-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aac69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="aac69-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aac69-119">Request headers</span></span>
|<span data-ttu-id="aac69-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aac69-120">Header</span></span>|<span data-ttu-id="aac69-121">Valor</span><span class="sxs-lookup"><span data-stu-id="aac69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aac69-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aac69-122">Authorization</span></span>|<span data-ttu-id="aac69-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aac69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aac69-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aac69-124">Accept</span></span>|<span data-ttu-id="aac69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aac69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aac69-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aac69-126">Request body</span></span>
<span data-ttu-id="aac69-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="aac69-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="aac69-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="aac69-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="aac69-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aac69-129">Property</span></span>|<span data-ttu-id="aac69-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="aac69-130">Type</span></span>|<span data-ttu-id="aac69-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="aac69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aac69-132">id</span><span class="sxs-lookup"><span data-stu-id="aac69-132">id</span></span>|<span data-ttu-id="aac69-133">String</span><span class="sxs-lookup"><span data-stu-id="aac69-133">String</span></span>|<span data-ttu-id="aac69-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aac69-134">Key of the entity.</span></span> <span data-ttu-id="aac69-135">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="aac69-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="aac69-136">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="aac69-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="aac69-137">displayName</span><span class="sxs-lookup"><span data-stu-id="aac69-137">displayName</span></span>|<span data-ttu-id="aac69-138">String</span><span class="sxs-lookup"><span data-stu-id="aac69-138">String</span></span>|<span data-ttu-id="aac69-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="aac69-139">Display Name of the Role definition.</span></span> <span data-ttu-id="aac69-140">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="aac69-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="aac69-141">description</span><span class="sxs-lookup"><span data-stu-id="aac69-141">description</span></span>|<span data-ttu-id="aac69-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aac69-142">String</span></span>|<span data-ttu-id="aac69-143">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="aac69-143">Description of the Role definition.</span></span> <span data-ttu-id="aac69-144">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="aac69-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="aac69-145">permissions</span><span class="sxs-lookup"><span data-stu-id="aac69-145">permissions</span></span>|<span data-ttu-id="aac69-146">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="aac69-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="aac69-147">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="aac69-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="aac69-148">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="aac69-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="aac69-149">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="aac69-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="aac69-150">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="aac69-150">rolePermissions</span></span>|<span data-ttu-id="aac69-151">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="aac69-151">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="aac69-152">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="aac69-152">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="aac69-153">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="aac69-153">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="aac69-154">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="aac69-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="aac69-155">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="aac69-155">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="aac69-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="aac69-156">Boolean</span></span>|<span data-ttu-id="aac69-157">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="aac69-157">Type of Role.</span></span> <span data-ttu-id="aac69-158">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="aac69-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="aac69-159">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="aac69-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="aac69-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="aac69-160">isBuiltIn</span></span>|<span data-ttu-id="aac69-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="aac69-161">Boolean</span></span>|<span data-ttu-id="aac69-162">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="aac69-162">Type of Role.</span></span> <span data-ttu-id="aac69-163">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="aac69-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="aac69-164">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="aac69-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="aac69-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aac69-165">roleScopeTagIds</span></span>|<span data-ttu-id="aac69-166">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aac69-166">String collection</span></span>|<span data-ttu-id="aac69-167">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="aac69-167">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aac69-168">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="aac69-168">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="aac69-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="aac69-169">Response</span></span>
<span data-ttu-id="aac69-170">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aac69-170">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac69-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aac69-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="aac69-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aac69-172">Request</span></span>
<span data-ttu-id="aac69-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aac69-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aac69-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="aac69-174">Response</span></span>
<span data-ttu-id="aac69-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aac69-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




