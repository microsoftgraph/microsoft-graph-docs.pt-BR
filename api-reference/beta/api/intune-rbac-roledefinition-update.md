---
title: Atualizar roleDefinition
description: Atualizar as propriedades de um objeto roleDefinition.
ms.openlocfilehash: debf63b5d0b7116a1e8d1f9274868d97c3cb8931
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033774"
---
# <a name="update-roledefinition"></a><span data-ttu-id="d4ccc-103">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d4ccc-103">Update roleDefinition</span></span>

> <span data-ttu-id="d4ccc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4ccc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4ccc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4ccc-107">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d4ccc-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4ccc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4ccc-108">Prerequisites</span></span>
<span data-ttu-id="d4ccc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4ccc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4ccc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4ccc-111">Permission type</span></span>|<span data-ttu-id="d4ccc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4ccc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4ccc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4ccc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4ccc-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4ccc-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d4ccc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4ccc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4ccc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-116">Not supported.</span></span>|
|<span data-ttu-id="d4ccc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4ccc-117">Application</span></span>|<span data-ttu-id="d4ccc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4ccc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4ccc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="d4ccc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4ccc-120">Request headers</span></span>
|<span data-ttu-id="d4ccc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4ccc-121">Header</span></span>|<span data-ttu-id="d4ccc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d4ccc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4ccc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4ccc-123">Authorization</span></span>|<span data-ttu-id="d4ccc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4ccc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4ccc-125">Accept</span></span>|<span data-ttu-id="d4ccc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4ccc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4ccc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4ccc-127">Request body</span></span>
<span data-ttu-id="d4ccc-128">No corpo da solicitação, forneça uma representação JSON do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d4ccc-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="d4ccc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d4ccc-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="d4ccc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4ccc-130">Property</span></span>|<span data-ttu-id="d4ccc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4ccc-131">Type</span></span>|<span data-ttu-id="d4ccc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4ccc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4ccc-133">id</span><span class="sxs-lookup"><span data-stu-id="d4ccc-133">id</span></span>|<span data-ttu-id="d4ccc-134">String</span><span class="sxs-lookup"><span data-stu-id="d4ccc-134">String</span></span>|<span data-ttu-id="d4ccc-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-135">Key of the entity.</span></span> <span data-ttu-id="d4ccc-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="d4ccc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d4ccc-137">displayName</span></span>|<span data-ttu-id="d4ccc-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4ccc-138">String</span></span>|<span data-ttu-id="d4ccc-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="d4ccc-140">description</span><span class="sxs-lookup"><span data-stu-id="d4ccc-140">description</span></span>|<span data-ttu-id="d4ccc-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4ccc-141">String</span></span>|<span data-ttu-id="d4ccc-142">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="d4ccc-143">permissions</span><span class="sxs-lookup"><span data-stu-id="d4ccc-143">permissions</span></span>|<span data-ttu-id="d4ccc-144">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="d4ccc-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="d4ccc-145">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="d4ccc-146">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="d4ccc-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="d4ccc-147">rolePermissions</span></span>|<span data-ttu-id="d4ccc-148">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="d4ccc-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="d4ccc-149">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="d4ccc-150">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="d4ccc-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d4ccc-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="d4ccc-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ccc-152">Boolean</span></span>|<span data-ttu-id="d4ccc-153">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-153">Type of Role.</span></span> <span data-ttu-id="d4ccc-154">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="d4ccc-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="d4ccc-155">isBuiltIn</span></span>|<span data-ttu-id="d4ccc-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ccc-156">Boolean</span></span>|<span data-ttu-id="d4ccc-157">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-157">Type of Role.</span></span> <span data-ttu-id="d4ccc-158">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="d4ccc-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4ccc-159">Response</span></span>
<span data-ttu-id="d4ccc-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-160">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4ccc-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4ccc-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4ccc-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4ccc-162">Request</span></span>
<span data-ttu-id="d4ccc-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1092

{
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
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="d4ccc-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4ccc-164">Response</span></span>
<span data-ttu-id="d4ccc-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4ccc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1194

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
  "isBuiltIn": true
}
```





