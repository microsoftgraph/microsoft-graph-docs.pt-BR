---
title: Criar roleDefinition
description: Criar um novo objeto roleDefinition
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f357beb705c2b61c7d7ed06dbaaf515dd9e934a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295961"
---
# <a name="create-roledefinition"></a><span data-ttu-id="2b85c-103">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2b85c-103">Create roleDefinition</span></span>

<span data-ttu-id="2b85c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b85c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b85c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b85c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b85c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b85c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b85c-107">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2b85c-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b85c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2b85c-108">Prerequisites</span></span>
<span data-ttu-id="2b85c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b85c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b85c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b85c-111">Permission type</span></span>|<span data-ttu-id="2b85c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2b85c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b85c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b85c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b85c-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b85c-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="2b85c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b85c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b85c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b85c-116">Not supported.</span></span>|
|<span data-ttu-id="2b85c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b85c-117">Application</span></span>|<span data-ttu-id="2b85c-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b85c-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b85c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b85c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="2b85c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b85c-120">Request headers</span></span>
|<span data-ttu-id="2b85c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b85c-121">Header</span></span>|<span data-ttu-id="2b85c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2b85c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b85c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b85c-123">Authorization</span></span>|<span data-ttu-id="2b85c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b85c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b85c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2b85c-125">Accept</span></span>|<span data-ttu-id="2b85c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b85c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b85c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b85c-127">Request body</span></span>
<span data-ttu-id="2b85c-128">No corpo da solicitação, forneça uma representação JSON do objeto roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="2b85c-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="2b85c-129">A tabela a seguir mostra as propriedades obrigatórias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="2b85c-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="2b85c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b85c-130">Property</span></span>|<span data-ttu-id="2b85c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b85c-131">Type</span></span>|<span data-ttu-id="2b85c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b85c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b85c-133">id</span><span class="sxs-lookup"><span data-stu-id="2b85c-133">id</span></span>|<span data-ttu-id="2b85c-134">String</span><span class="sxs-lookup"><span data-stu-id="2b85c-134">String</span></span>|<span data-ttu-id="2b85c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2b85c-135">Key of the entity.</span></span> <span data-ttu-id="2b85c-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="2b85c-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="2b85c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2b85c-137">displayName</span></span>|<span data-ttu-id="2b85c-138">String</span><span class="sxs-lookup"><span data-stu-id="2b85c-138">String</span></span>|<span data-ttu-id="2b85c-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="2b85c-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="2b85c-140">description</span><span class="sxs-lookup"><span data-stu-id="2b85c-140">description</span></span>|<span data-ttu-id="2b85c-141">String</span><span class="sxs-lookup"><span data-stu-id="2b85c-141">String</span></span>|<span data-ttu-id="2b85c-142">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="2b85c-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="2b85c-143">permissões</span><span class="sxs-lookup"><span data-stu-id="2b85c-143">permissions</span></span>|<span data-ttu-id="2b85c-144">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="2b85c-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="2b85c-145">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="2b85c-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="2b85c-146">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="2b85c-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="2b85c-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="2b85c-147">rolePermissions</span></span>|<span data-ttu-id="2b85c-148">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="2b85c-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="2b85c-149">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="2b85c-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="2b85c-150">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="2b85c-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="2b85c-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2b85c-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="2b85c-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="2b85c-152">Boolean</span></span>|<span data-ttu-id="2b85c-153">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="2b85c-153">Type of Role.</span></span> <span data-ttu-id="2b85c-154">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="2b85c-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="2b85c-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="2b85c-155">isBuiltIn</span></span>|<span data-ttu-id="2b85c-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="2b85c-156">Boolean</span></span>|<span data-ttu-id="2b85c-157">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="2b85c-157">Type of Role.</span></span> <span data-ttu-id="2b85c-158">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="2b85c-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="2b85c-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b85c-159">roleScopeTagIds</span></span>|<span data-ttu-id="2b85c-160">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b85c-160">String collection</span></span>|<span data-ttu-id="2b85c-161">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2b85c-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="2b85c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b85c-162">Response</span></span>
<span data-ttu-id="2b85c-163">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b85c-163">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b85c-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b85c-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b85c-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b85c-165">Request</span></span>
<span data-ttu-id="2b85c-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b85c-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b85c-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b85c-167">Response</span></span>
<span data-ttu-id="2b85c-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b85c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




