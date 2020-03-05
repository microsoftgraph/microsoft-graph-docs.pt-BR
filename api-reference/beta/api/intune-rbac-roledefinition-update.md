---
title: Atualizar roleDefinition
description: Atualizar as propriedades de um objeto roleDefinition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e05136a24bbac8d9b646ea3b213884ca77355782
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459636"
---
# <a name="update-roledefinition"></a><span data-ttu-id="37b05-103">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="37b05-103">Update roleDefinition</span></span>

<span data-ttu-id="37b05-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="37b05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37b05-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37b05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37b05-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37b05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37b05-107">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="37b05-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37b05-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37b05-108">Prerequisites</span></span>
<span data-ttu-id="37b05-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37b05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37b05-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37b05-111">Permission type</span></span>|<span data-ttu-id="37b05-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37b05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37b05-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37b05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37b05-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37b05-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="37b05-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37b05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37b05-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37b05-116">Not supported.</span></span>|
|<span data-ttu-id="37b05-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37b05-117">Application</span></span>|<span data-ttu-id="37b05-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37b05-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37b05-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37b05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="37b05-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37b05-120">Request headers</span></span>
|<span data-ttu-id="37b05-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37b05-121">Header</span></span>|<span data-ttu-id="37b05-122">Valor</span><span class="sxs-lookup"><span data-stu-id="37b05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37b05-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="37b05-123">Authorization</span></span>|<span data-ttu-id="37b05-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37b05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37b05-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37b05-125">Accept</span></span>|<span data-ttu-id="37b05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37b05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37b05-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37b05-127">Request body</span></span>
<span data-ttu-id="37b05-128">No corpo da solicitação, forneça uma representação JSON do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="37b05-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="37b05-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="37b05-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="37b05-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37b05-130">Property</span></span>|<span data-ttu-id="37b05-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="37b05-131">Type</span></span>|<span data-ttu-id="37b05-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="37b05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37b05-133">id</span><span class="sxs-lookup"><span data-stu-id="37b05-133">id</span></span>|<span data-ttu-id="37b05-134">String</span><span class="sxs-lookup"><span data-stu-id="37b05-134">String</span></span>|<span data-ttu-id="37b05-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="37b05-135">Key of the entity.</span></span> <span data-ttu-id="37b05-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="37b05-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="37b05-137">displayName</span><span class="sxs-lookup"><span data-stu-id="37b05-137">displayName</span></span>|<span data-ttu-id="37b05-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37b05-138">String</span></span>|<span data-ttu-id="37b05-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="37b05-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="37b05-140">description</span><span class="sxs-lookup"><span data-stu-id="37b05-140">description</span></span>|<span data-ttu-id="37b05-141">String</span><span class="sxs-lookup"><span data-stu-id="37b05-141">String</span></span>|<span data-ttu-id="37b05-142">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="37b05-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="37b05-143">permissões</span><span class="sxs-lookup"><span data-stu-id="37b05-143">permissions</span></span>|<span data-ttu-id="37b05-144">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="37b05-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="37b05-145">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="37b05-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="37b05-146">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="37b05-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="37b05-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="37b05-147">rolePermissions</span></span>|<span data-ttu-id="37b05-148">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="37b05-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="37b05-149">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="37b05-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="37b05-150">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="37b05-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="37b05-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="37b05-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="37b05-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="37b05-152">Boolean</span></span>|<span data-ttu-id="37b05-153">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="37b05-153">Type of Role.</span></span> <span data-ttu-id="37b05-154">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="37b05-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="37b05-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="37b05-155">isBuiltIn</span></span>|<span data-ttu-id="37b05-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="37b05-156">Boolean</span></span>|<span data-ttu-id="37b05-157">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="37b05-157">Type of Role.</span></span> <span data-ttu-id="37b05-158">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="37b05-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="37b05-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="37b05-159">roleScopeTagIds</span></span>|<span data-ttu-id="37b05-160">String collection</span><span class="sxs-lookup"><span data-stu-id="37b05-160">String collection</span></span>|<span data-ttu-id="37b05-161">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="37b05-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="37b05-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="37b05-162">Response</span></span>
<span data-ttu-id="37b05-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37b05-163">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37b05-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37b05-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="37b05-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37b05-165">Request</span></span>
<span data-ttu-id="37b05-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37b05-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37b05-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="37b05-167">Response</span></span>
<span data-ttu-id="37b05-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37b05-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





