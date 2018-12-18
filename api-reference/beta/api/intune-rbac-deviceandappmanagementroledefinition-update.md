---
title: Atualizar deviceAndAppManagementRoleDefinition
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleDefinition.
author: tfitzmac
ms.openlocfilehash: ee118a2593a968557f8ccf9103d6f50af014a491
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362801"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="255ab-103">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="255ab-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="255ab-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="255ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="255ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="255ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="255ab-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="255ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="255ab-107">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="255ab-107">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="255ab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="255ab-108">Prerequisites</span></span>
<span data-ttu-id="255ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="255ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="255ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="255ab-111">Permission type</span></span>|<span data-ttu-id="255ab-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="255ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="255ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="255ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="255ab-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="255ab-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="255ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="255ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="255ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="255ab-116">Not supported.</span></span>|
|<span data-ttu-id="255ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="255ab-117">Application</span></span>|<span data-ttu-id="255ab-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="255ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="255ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="255ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="255ab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="255ab-120">Request headers</span></span>
|<span data-ttu-id="255ab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="255ab-121">Header</span></span>|<span data-ttu-id="255ab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="255ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="255ab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="255ab-123">Authorization</span></span>|<span data-ttu-id="255ab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="255ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="255ab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="255ab-125">Accept</span></span>|<span data-ttu-id="255ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="255ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="255ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="255ab-127">Request body</span></span>
<span data-ttu-id="255ab-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="255ab-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="255ab-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="255ab-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="255ab-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="255ab-130">Property</span></span>|<span data-ttu-id="255ab-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="255ab-131">Type</span></span>|<span data-ttu-id="255ab-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="255ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="255ab-133">id</span><span class="sxs-lookup"><span data-stu-id="255ab-133">id</span></span>|<span data-ttu-id="255ab-134">String</span><span class="sxs-lookup"><span data-stu-id="255ab-134">String</span></span>|<span data-ttu-id="255ab-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="255ab-135">Key of the entity.</span></span> <span data-ttu-id="255ab-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="255ab-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="255ab-137">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="255ab-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="255ab-138">displayName</span><span class="sxs-lookup"><span data-stu-id="255ab-138">displayName</span></span>|<span data-ttu-id="255ab-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="255ab-139">String</span></span>|<span data-ttu-id="255ab-140">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="255ab-140">Display Name of the Role definition.</span></span> <span data-ttu-id="255ab-141">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="255ab-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="255ab-142">description</span><span class="sxs-lookup"><span data-stu-id="255ab-142">description</span></span>|<span data-ttu-id="255ab-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="255ab-143">String</span></span>|<span data-ttu-id="255ab-144">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="255ab-144">Description of the Role definition.</span></span> <span data-ttu-id="255ab-145">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="255ab-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="255ab-146">permissions</span><span class="sxs-lookup"><span data-stu-id="255ab-146">permissions</span></span>|<span data-ttu-id="255ab-147">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="255ab-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="255ab-148">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="255ab-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="255ab-149">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="255ab-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="255ab-150">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="255ab-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="255ab-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="255ab-151">rolePermissions</span></span>|<span data-ttu-id="255ab-152">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="255ab-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="255ab-153">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="255ab-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="255ab-154">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="255ab-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="255ab-155">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="255ab-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="255ab-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="255ab-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="255ab-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="255ab-157">Boolean</span></span>|<span data-ttu-id="255ab-158">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="255ab-158">Type of Role.</span></span> <span data-ttu-id="255ab-159">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="255ab-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="255ab-160">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="255ab-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="255ab-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="255ab-161">isBuiltIn</span></span>|<span data-ttu-id="255ab-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="255ab-162">Boolean</span></span>|<span data-ttu-id="255ab-163">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="255ab-163">Type of Role.</span></span> <span data-ttu-id="255ab-164">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="255ab-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="255ab-165">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="255ab-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="255ab-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="255ab-166">Response</span></span>
<span data-ttu-id="255ab-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="255ab-167">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="255ab-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="255ab-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="255ab-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="255ab-169">Request</span></span>
<span data-ttu-id="255ab-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="255ab-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="255ab-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="255ab-171">Response</span></span>
<span data-ttu-id="255ab-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="255ab-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1216

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
  "isBuiltIn": true
}
```





