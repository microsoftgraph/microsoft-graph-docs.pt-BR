---
title: Atualizar roleDefinition
description: Atualizar as propriedades de um objeto roleDefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b13f82e30e8bf67a78bd31db678de5b5a46051c3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412622"
---
# <a name="update-roledefinition"></a><span data-ttu-id="ef79b-103">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="ef79b-103">Update roleDefinition</span></span>

> <span data-ttu-id="ef79b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ef79b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ef79b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ef79b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef79b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ef79b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef79b-107">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ef79b-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef79b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef79b-108">Prerequisites</span></span>
<span data-ttu-id="ef79b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ef79b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ef79b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef79b-111">Permission type</span></span>|<span data-ttu-id="ef79b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef79b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef79b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef79b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef79b-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef79b-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ef79b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef79b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef79b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef79b-116">Not supported.</span></span>|
|<span data-ttu-id="ef79b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef79b-117">Application</span></span>|<span data-ttu-id="ef79b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef79b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef79b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef79b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="ef79b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef79b-120">Request headers</span></span>
|<span data-ttu-id="ef79b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef79b-121">Header</span></span>|<span data-ttu-id="ef79b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef79b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef79b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef79b-123">Authorization</span></span>|<span data-ttu-id="ef79b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef79b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef79b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef79b-125">Accept</span></span>|<span data-ttu-id="ef79b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef79b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef79b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef79b-127">Request body</span></span>
<span data-ttu-id="ef79b-128">No corpo da solicitação, forneça uma representação JSON do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ef79b-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="ef79b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ef79b-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="ef79b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef79b-130">Property</span></span>|<span data-ttu-id="ef79b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef79b-131">Type</span></span>|<span data-ttu-id="ef79b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef79b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef79b-133">id</span><span class="sxs-lookup"><span data-stu-id="ef79b-133">id</span></span>|<span data-ttu-id="ef79b-134">String</span><span class="sxs-lookup"><span data-stu-id="ef79b-134">String</span></span>|<span data-ttu-id="ef79b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ef79b-135">Key of the entity.</span></span> <span data-ttu-id="ef79b-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="ef79b-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="ef79b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ef79b-137">displayName</span></span>|<span data-ttu-id="ef79b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef79b-138">String</span></span>|<span data-ttu-id="ef79b-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="ef79b-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="ef79b-140">description</span><span class="sxs-lookup"><span data-stu-id="ef79b-140">description</span></span>|<span data-ttu-id="ef79b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef79b-141">String</span></span>|<span data-ttu-id="ef79b-142">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="ef79b-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="ef79b-143">permissions</span><span class="sxs-lookup"><span data-stu-id="ef79b-143">permissions</span></span>|<span data-ttu-id="ef79b-144">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ef79b-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ef79b-145">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="ef79b-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ef79b-146">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="ef79b-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="ef79b-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ef79b-147">rolePermissions</span></span>|<span data-ttu-id="ef79b-148">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ef79b-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ef79b-149">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="ef79b-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ef79b-150">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="ef79b-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="ef79b-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ef79b-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="ef79b-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef79b-152">Boolean</span></span>|<span data-ttu-id="ef79b-153">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="ef79b-153">Type of Role.</span></span> <span data-ttu-id="ef79b-154">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="ef79b-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="ef79b-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ef79b-155">isBuiltIn</span></span>|<span data-ttu-id="ef79b-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef79b-156">Boolean</span></span>|<span data-ttu-id="ef79b-157">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="ef79b-157">Type of Role.</span></span> <span data-ttu-id="ef79b-158">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="ef79b-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="ef79b-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef79b-159">roleScopeTagIds</span></span>|<span data-ttu-id="ef79b-160">String collection</span><span class="sxs-lookup"><span data-stu-id="ef79b-160">String collection</span></span>|<span data-ttu-id="ef79b-161">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="ef79b-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="ef79b-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef79b-162">Response</span></span>
<span data-ttu-id="ef79b-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef79b-163">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef79b-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef79b-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef79b-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef79b-165">Request</span></span>
<span data-ttu-id="ef79b-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef79b-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef79b-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef79b-167">Response</span></span>
<span data-ttu-id="ef79b-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef79b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




