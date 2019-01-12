---
title: Atualizar deviceAndAppManagementRoleDefinition
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 102c4c024d02977351f4b7eb6e3586141b3ff3d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933600"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="6bac3-103">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6bac3-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="6bac3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6bac3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bac3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6bac3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bac3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6bac3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bac3-107">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6bac3-107">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6bac3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6bac3-108">Prerequisites</span></span>
<span data-ttu-id="6bac3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bac3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bac3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bac3-111">Permission type</span></span>|<span data-ttu-id="6bac3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6bac3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bac3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bac3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6bac3-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bac3-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="6bac3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bac3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bac3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bac3-116">Not supported.</span></span>|
|<span data-ttu-id="6bac3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bac3-117">Application</span></span>|<span data-ttu-id="6bac3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bac3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bac3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bac3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="6bac3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bac3-120">Request headers</span></span>
|<span data-ttu-id="6bac3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6bac3-121">Header</span></span>|<span data-ttu-id="6bac3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6bac3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bac3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bac3-123">Authorization</span></span>|<span data-ttu-id="6bac3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bac3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bac3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6bac3-125">Accept</span></span>|<span data-ttu-id="6bac3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6bac3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bac3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bac3-127">Request body</span></span>
<span data-ttu-id="6bac3-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6bac3-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="6bac3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6bac3-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="6bac3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bac3-130">Property</span></span>|<span data-ttu-id="6bac3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bac3-131">Type</span></span>|<span data-ttu-id="6bac3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bac3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bac3-133">id</span><span class="sxs-lookup"><span data-stu-id="6bac3-133">id</span></span>|<span data-ttu-id="6bac3-134">String</span><span class="sxs-lookup"><span data-stu-id="6bac3-134">String</span></span>|<span data-ttu-id="6bac3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6bac3-135">Key of the entity.</span></span> <span data-ttu-id="6bac3-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="6bac3-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="6bac3-137">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6bac3-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6bac3-138">displayName</span><span class="sxs-lookup"><span data-stu-id="6bac3-138">displayName</span></span>|<span data-ttu-id="6bac3-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bac3-139">String</span></span>|<span data-ttu-id="6bac3-140">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="6bac3-140">Display Name of the Role definition.</span></span> <span data-ttu-id="6bac3-141">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6bac3-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6bac3-142">description</span><span class="sxs-lookup"><span data-stu-id="6bac3-142">description</span></span>|<span data-ttu-id="6bac3-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bac3-143">String</span></span>|<span data-ttu-id="6bac3-144">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="6bac3-144">Description of the Role definition.</span></span> <span data-ttu-id="6bac3-145">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6bac3-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6bac3-146">permissions</span><span class="sxs-lookup"><span data-stu-id="6bac3-146">permissions</span></span>|<span data-ttu-id="6bac3-147">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="6bac3-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="6bac3-148">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="6bac3-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="6bac3-149">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="6bac3-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="6bac3-150">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6bac3-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6bac3-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="6bac3-151">rolePermissions</span></span>|<span data-ttu-id="6bac3-152">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="6bac3-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="6bac3-153">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="6bac3-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="6bac3-154">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="6bac3-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="6bac3-155">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6bac3-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6bac3-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="6bac3-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="6bac3-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="6bac3-157">Boolean</span></span>|<span data-ttu-id="6bac3-158">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="6bac3-158">Type of Role.</span></span> <span data-ttu-id="6bac3-159">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="6bac3-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="6bac3-160">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6bac3-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="6bac3-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="6bac3-161">isBuiltIn</span></span>|<span data-ttu-id="6bac3-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="6bac3-162">Boolean</span></span>|<span data-ttu-id="6bac3-163">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="6bac3-163">Type of Role.</span></span> <span data-ttu-id="6bac3-164">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="6bac3-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="6bac3-165">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="6bac3-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6bac3-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bac3-166">Response</span></span>
<span data-ttu-id="6bac3-167">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bac3-167">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bac3-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bac3-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="6bac3-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bac3-169">Request</span></span>
<span data-ttu-id="6bac3-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bac3-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6bac3-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bac3-171">Response</span></span>
<span data-ttu-id="6bac3-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bac3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





