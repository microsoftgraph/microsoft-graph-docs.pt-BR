---
title: Criar deviceAndAppManagementRoleDefinition
description: Cria um novo objeto deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bcc3287c396051c4ed385bf3759b08f68fb54b01
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210897"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="369eb-103">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="369eb-103">Create deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="369eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="369eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="369eb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="369eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="369eb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="369eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="369eb-107">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="369eb-107">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="369eb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="369eb-108">Prerequisites</span></span>
<span data-ttu-id="369eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="369eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="369eb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="369eb-111">Permission type</span></span>|<span data-ttu-id="369eb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="369eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="369eb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="369eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="369eb-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="369eb-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="369eb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="369eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="369eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="369eb-116">Not supported.</span></span>|
|<span data-ttu-id="369eb-117">Application</span><span class="sxs-lookup"><span data-stu-id="369eb-117">Application</span></span>|<span data-ttu-id="369eb-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="369eb-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="369eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="369eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="369eb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="369eb-120">Request headers</span></span>
|<span data-ttu-id="369eb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="369eb-121">Header</span></span>|<span data-ttu-id="369eb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="369eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="369eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="369eb-123">Authorization</span></span>|<span data-ttu-id="369eb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="369eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="369eb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="369eb-125">Accept</span></span>|<span data-ttu-id="369eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="369eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="369eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="369eb-127">Request body</span></span>
<span data-ttu-id="369eb-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="369eb-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="369eb-129">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="369eb-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="369eb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="369eb-130">Property</span></span>|<span data-ttu-id="369eb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="369eb-131">Type</span></span>|<span data-ttu-id="369eb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="369eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="369eb-133">id</span><span class="sxs-lookup"><span data-stu-id="369eb-133">id</span></span>|<span data-ttu-id="369eb-134">String</span><span class="sxs-lookup"><span data-stu-id="369eb-134">String</span></span>|<span data-ttu-id="369eb-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="369eb-135">Key of the entity.</span></span> <span data-ttu-id="369eb-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="369eb-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="369eb-137">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="369eb-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="369eb-138">displayName</span><span class="sxs-lookup"><span data-stu-id="369eb-138">displayName</span></span>|<span data-ttu-id="369eb-139">String</span><span class="sxs-lookup"><span data-stu-id="369eb-139">String</span></span>|<span data-ttu-id="369eb-140">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="369eb-140">Display Name of the Role definition.</span></span> <span data-ttu-id="369eb-141">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="369eb-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="369eb-142">description</span><span class="sxs-lookup"><span data-stu-id="369eb-142">description</span></span>|<span data-ttu-id="369eb-143">String</span><span class="sxs-lookup"><span data-stu-id="369eb-143">String</span></span>|<span data-ttu-id="369eb-144">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="369eb-144">Description of the Role definition.</span></span> <span data-ttu-id="369eb-145">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="369eb-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="369eb-146">permissões</span><span class="sxs-lookup"><span data-stu-id="369eb-146">permissions</span></span>|<span data-ttu-id="369eb-147">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="369eb-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="369eb-148">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="369eb-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="369eb-149">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="369eb-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="369eb-150">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="369eb-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="369eb-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="369eb-151">rolePermissions</span></span>|<span data-ttu-id="369eb-152">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="369eb-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="369eb-153">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="369eb-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="369eb-154">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="369eb-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="369eb-155">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="369eb-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="369eb-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="369eb-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="369eb-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="369eb-157">Boolean</span></span>|<span data-ttu-id="369eb-158">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="369eb-158">Type of Role.</span></span> <span data-ttu-id="369eb-159">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="369eb-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="369eb-160">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="369eb-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="369eb-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="369eb-161">isBuiltIn</span></span>|<span data-ttu-id="369eb-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="369eb-162">Boolean</span></span>|<span data-ttu-id="369eb-163">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="369eb-163">Type of Role.</span></span> <span data-ttu-id="369eb-164">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="369eb-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="369eb-165">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="369eb-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="369eb-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="369eb-166">roleScopeTagIds</span></span>|<span data-ttu-id="369eb-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="369eb-167">String collection</span></span>|<span data-ttu-id="369eb-168">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="369eb-168">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="369eb-169">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="369eb-169">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="369eb-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="369eb-170">Response</span></span>
<span data-ttu-id="369eb-171">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="369eb-171">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="369eb-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="369eb-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="369eb-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="369eb-173">Request</span></span>
<span data-ttu-id="369eb-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="369eb-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="369eb-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="369eb-175">Response</span></span>
<span data-ttu-id="369eb-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="369eb-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




