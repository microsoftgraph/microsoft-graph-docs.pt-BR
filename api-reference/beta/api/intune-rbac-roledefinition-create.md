---
title: Criar roleDefinition
description: Criar um novo objeto roleDefinition
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3f23888e92909c629a7b91f010d64f9e184f0b5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960192"
---
# <a name="create-roledefinition"></a><span data-ttu-id="73518-103">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="73518-103">Create roleDefinition</span></span>

> <span data-ttu-id="73518-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73518-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73518-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73518-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73518-106">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="73518-106">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73518-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73518-107">Prerequisites</span></span>
<span data-ttu-id="73518-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73518-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73518-110">Permission type</span></span>|<span data-ttu-id="73518-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73518-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73518-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73518-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73518-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73518-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="73518-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73518-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73518-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73518-115">Not supported.</span></span>|
|<span data-ttu-id="73518-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73518-116">Application</span></span>|<span data-ttu-id="73518-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73518-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73518-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73518-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="73518-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73518-119">Request headers</span></span>
|<span data-ttu-id="73518-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73518-120">Header</span></span>|<span data-ttu-id="73518-121">Valor</span><span class="sxs-lookup"><span data-stu-id="73518-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73518-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73518-122">Authorization</span></span>|<span data-ttu-id="73518-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73518-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73518-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73518-124">Accept</span></span>|<span data-ttu-id="73518-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73518-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73518-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73518-126">Request body</span></span>
<span data-ttu-id="73518-127">No corpo da solicitação, forneça uma representação JSON do objeto roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="73518-127">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="73518-128">A tabela a seguir mostra as propriedades obrigatórias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="73518-128">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="73518-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73518-129">Property</span></span>|<span data-ttu-id="73518-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="73518-130">Type</span></span>|<span data-ttu-id="73518-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="73518-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73518-132">id</span><span class="sxs-lookup"><span data-stu-id="73518-132">id</span></span>|<span data-ttu-id="73518-133">String</span><span class="sxs-lookup"><span data-stu-id="73518-133">String</span></span>|<span data-ttu-id="73518-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="73518-134">Key of the entity.</span></span> <span data-ttu-id="73518-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="73518-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="73518-136">displayName</span><span class="sxs-lookup"><span data-stu-id="73518-136">displayName</span></span>|<span data-ttu-id="73518-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73518-137">String</span></span>|<span data-ttu-id="73518-138">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="73518-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="73518-139">descrição</span><span class="sxs-lookup"><span data-stu-id="73518-139">description</span></span>|<span data-ttu-id="73518-140">String</span><span class="sxs-lookup"><span data-stu-id="73518-140">String</span></span>|<span data-ttu-id="73518-141">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="73518-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="73518-142">permissões</span><span class="sxs-lookup"><span data-stu-id="73518-142">permissions</span></span>|<span data-ttu-id="73518-143">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="73518-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="73518-144">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="73518-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="73518-145">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="73518-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="73518-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="73518-146">rolePermissions</span></span>|<span data-ttu-id="73518-147">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="73518-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="73518-148">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="73518-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="73518-149">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="73518-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="73518-150">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="73518-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="73518-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="73518-151">Boolean</span></span>|<span data-ttu-id="73518-152">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="73518-152">Type of Role.</span></span> <span data-ttu-id="73518-153">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="73518-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="73518-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="73518-154">isBuiltIn</span></span>|<span data-ttu-id="73518-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="73518-155">Boolean</span></span>|<span data-ttu-id="73518-156">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="73518-156">Type of Role.</span></span> <span data-ttu-id="73518-157">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="73518-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="73518-158">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73518-158">roleScopeTagIds</span></span>|<span data-ttu-id="73518-159">Coleção String</span><span class="sxs-lookup"><span data-stu-id="73518-159">String collection</span></span>|<span data-ttu-id="73518-160">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="73518-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="73518-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="73518-161">Response</span></span>
<span data-ttu-id="73518-162">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73518-162">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73518-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73518-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="73518-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73518-164">Request</span></span>
<span data-ttu-id="73518-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73518-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="73518-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="73518-166">Response</span></span>
<span data-ttu-id="73518-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73518-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




