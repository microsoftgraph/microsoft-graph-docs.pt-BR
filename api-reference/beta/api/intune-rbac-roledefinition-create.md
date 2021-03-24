---
title: Criar roleDefinition
description: Criar um novo objeto roleDefinition
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f7d31dd9dab0219af303c5d03950fd572d8ebc1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141586"
---
# <a name="create-roledefinition"></a><span data-ttu-id="c897b-103">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c897b-103">Create roleDefinition</span></span>

<span data-ttu-id="c897b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c897b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c897b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c897b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c897b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c897b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c897b-107">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c897b-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c897b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c897b-108">Prerequisites</span></span>
<span data-ttu-id="c897b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c897b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c897b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c897b-111">Permission type</span></span>|<span data-ttu-id="c897b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c897b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c897b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c897b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c897b-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c897b-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c897b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c897b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c897b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c897b-116">Not supported.</span></span>|
|<span data-ttu-id="c897b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c897b-117">Application</span></span>|<span data-ttu-id="c897b-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c897b-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c897b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c897b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="c897b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c897b-120">Request headers</span></span>
|<span data-ttu-id="c897b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c897b-121">Header</span></span>|<span data-ttu-id="c897b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c897b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c897b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c897b-123">Authorization</span></span>|<span data-ttu-id="c897b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c897b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c897b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c897b-125">Accept</span></span>|<span data-ttu-id="c897b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c897b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c897b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c897b-127">Request body</span></span>
<span data-ttu-id="c897b-128">No corpo da solicitação, forneça uma representação JSON do objeto roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="c897b-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="c897b-129">A tabela a seguir mostra as propriedades obrigatórias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="c897b-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="c897b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c897b-130">Property</span></span>|<span data-ttu-id="c897b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c897b-131">Type</span></span>|<span data-ttu-id="c897b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c897b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c897b-133">id</span><span class="sxs-lookup"><span data-stu-id="c897b-133">id</span></span>|<span data-ttu-id="c897b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c897b-134">String</span></span>|<span data-ttu-id="c897b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c897b-135">Key of the entity.</span></span> <span data-ttu-id="c897b-136">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c897b-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="c897b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c897b-137">displayName</span></span>|<span data-ttu-id="c897b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c897b-138">String</span></span>|<span data-ttu-id="c897b-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="c897b-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="c897b-140">descrição</span><span class="sxs-lookup"><span data-stu-id="c897b-140">description</span></span>|<span data-ttu-id="c897b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c897b-141">String</span></span>|<span data-ttu-id="c897b-142">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="c897b-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="c897b-143">permissões</span><span class="sxs-lookup"><span data-stu-id="c897b-143">permissions</span></span>|<span data-ttu-id="c897b-144">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="c897b-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c897b-145">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="c897b-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c897b-146">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="c897b-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="c897b-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="c897b-147">rolePermissions</span></span>|<span data-ttu-id="c897b-148">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="c897b-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c897b-149">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="c897b-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c897b-150">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="c897b-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="c897b-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c897b-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="c897b-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="c897b-152">Boolean</span></span>|<span data-ttu-id="c897b-153">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="c897b-153">Type of Role.</span></span> <span data-ttu-id="c897b-154">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="c897b-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="c897b-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="c897b-155">isBuiltIn</span></span>|<span data-ttu-id="c897b-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="c897b-156">Boolean</span></span>|<span data-ttu-id="c897b-157">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="c897b-157">Type of Role.</span></span> <span data-ttu-id="c897b-158">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="c897b-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="c897b-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c897b-159">roleScopeTagIds</span></span>|<span data-ttu-id="c897b-160">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c897b-160">String collection</span></span>|<span data-ttu-id="c897b-161">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="c897b-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="c897b-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c897b-162">Response</span></span>
<span data-ttu-id="c897b-163">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c897b-163">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c897b-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c897b-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="c897b-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c897b-165">Request</span></span>
<span data-ttu-id="c897b-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c897b-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c897b-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="c897b-167">Response</span></span>
<span data-ttu-id="c897b-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c897b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




