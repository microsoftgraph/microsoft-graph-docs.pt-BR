---
title: Criar roleDefinition
description: Criar um novo objeto roleDefinition
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a274621d13246cbbbe7071353fa7126ea3568d47
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412657"
---
# <a name="create-roledefinition"></a><span data-ttu-id="dcbb0-103">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dcbb0-103">Create roleDefinition</span></span>

> <span data-ttu-id="dcbb0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dcbb0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dcbb0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcbb0-107">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dcbb0-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcbb0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dcbb0-108">Prerequisites</span></span>
<span data-ttu-id="dcbb0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dcbb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dcbb0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcbb0-111">Permission type</span></span>|<span data-ttu-id="dcbb0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dcbb0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcbb0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcbb0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dcbb0-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcbb0-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="dcbb0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcbb0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcbb0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-116">Not supported.</span></span>|
|<span data-ttu-id="dcbb0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcbb0-117">Application</span></span>|<span data-ttu-id="dcbb0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcbb0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcbb0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="dcbb0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbb0-120">Request headers</span></span>
|<span data-ttu-id="dcbb0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dcbb0-121">Header</span></span>|<span data-ttu-id="dcbb0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dcbb0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcbb0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcbb0-123">Authorization</span></span>|<span data-ttu-id="dcbb0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcbb0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dcbb0-125">Accept</span></span>|<span data-ttu-id="dcbb0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dcbb0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcbb0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbb0-127">Request body</span></span>
<span data-ttu-id="dcbb0-128">No corpo da solicitação, forneça uma representação JSON do objeto roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="dcbb0-129">A tabela a seguir mostra as propriedades obrigatórias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="dcbb0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dcbb0-130">Property</span></span>|<span data-ttu-id="dcbb0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcbb0-131">Type</span></span>|<span data-ttu-id="dcbb0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcbb0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcbb0-133">id</span><span class="sxs-lookup"><span data-stu-id="dcbb0-133">id</span></span>|<span data-ttu-id="dcbb0-134">String</span><span class="sxs-lookup"><span data-stu-id="dcbb0-134">String</span></span>|<span data-ttu-id="dcbb0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-135">Key of the entity.</span></span> <span data-ttu-id="dcbb0-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="dcbb0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="dcbb0-137">displayName</span></span>|<span data-ttu-id="dcbb0-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dcbb0-138">String</span></span>|<span data-ttu-id="dcbb0-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="dcbb0-140">description</span><span class="sxs-lookup"><span data-stu-id="dcbb0-140">description</span></span>|<span data-ttu-id="dcbb0-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dcbb0-141">String</span></span>|<span data-ttu-id="dcbb0-142">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="dcbb0-143">permissions</span><span class="sxs-lookup"><span data-stu-id="dcbb0-143">permissions</span></span>|<span data-ttu-id="dcbb0-144">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="dcbb0-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="dcbb0-145">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="dcbb0-146">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="dcbb0-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="dcbb0-147">rolePermissions</span></span>|<span data-ttu-id="dcbb0-148">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="dcbb0-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="dcbb0-149">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="dcbb0-150">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="dcbb0-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="dcbb0-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="dcbb0-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="dcbb0-152">Boolean</span></span>|<span data-ttu-id="dcbb0-153">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-153">Type of Role.</span></span> <span data-ttu-id="dcbb0-154">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="dcbb0-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="dcbb0-155">isBuiltIn</span></span>|<span data-ttu-id="dcbb0-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="dcbb0-156">Boolean</span></span>|<span data-ttu-id="dcbb0-157">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-157">Type of Role.</span></span> <span data-ttu-id="dcbb0-158">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="dcbb0-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dcbb0-159">roleScopeTagIds</span></span>|<span data-ttu-id="dcbb0-160">String collection</span><span class="sxs-lookup"><span data-stu-id="dcbb0-160">String collection</span></span>|<span data-ttu-id="dcbb0-161">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="dcbb0-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcbb0-162">Response</span></span>
<span data-ttu-id="dcbb0-163">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-163">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcbb0-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcbb0-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcbb0-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbb0-165">Request</span></span>
<span data-ttu-id="dcbb0-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dcbb0-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcbb0-167">Response</span></span>
<span data-ttu-id="dcbb0-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcbb0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




