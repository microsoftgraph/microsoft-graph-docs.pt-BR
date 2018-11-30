---
title: Criar roleDefinition
description: Criar um novo objeto roleDefinition
ms.openlocfilehash: 6772b065e4d4d73615540667470829b31a2de804
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041180"
---
# <a name="create-roledefinition"></a><span data-ttu-id="3b04d-103">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3b04d-103">Create roleDefinition</span></span>

> <span data-ttu-id="3b04d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3b04d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b04d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3b04d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b04d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3b04d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b04d-107">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b04d-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b04d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b04d-108">Prerequisites</span></span>
<span data-ttu-id="3b04d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b04d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b04d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b04d-111">Permission type</span></span>|<span data-ttu-id="3b04d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b04d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b04d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b04d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b04d-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b04d-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3b04d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b04d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b04d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b04d-116">Not supported.</span></span>|
|<span data-ttu-id="3b04d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b04d-117">Application</span></span>|<span data-ttu-id="3b04d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b04d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b04d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b04d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="3b04d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b04d-120">Request headers</span></span>
|<span data-ttu-id="3b04d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b04d-121">Header</span></span>|<span data-ttu-id="3b04d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3b04d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b04d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b04d-123">Authorization</span></span>|<span data-ttu-id="3b04d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b04d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b04d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b04d-125">Accept</span></span>|<span data-ttu-id="3b04d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b04d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b04d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b04d-127">Request body</span></span>
<span data-ttu-id="3b04d-128">No corpo da solicitação, forneça uma representação JSON do objeto roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="3b04d-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="3b04d-129">A tabela a seguir mostra as propriedades obrigatórias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="3b04d-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="3b04d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b04d-130">Property</span></span>|<span data-ttu-id="3b04d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b04d-131">Type</span></span>|<span data-ttu-id="3b04d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b04d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b04d-133">id</span><span class="sxs-lookup"><span data-stu-id="3b04d-133">id</span></span>|<span data-ttu-id="3b04d-134">String</span><span class="sxs-lookup"><span data-stu-id="3b04d-134">String</span></span>|<span data-ttu-id="3b04d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3b04d-135">Key of the entity.</span></span> <span data-ttu-id="3b04d-136">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3b04d-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="3b04d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3b04d-137">displayName</span></span>|<span data-ttu-id="3b04d-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b04d-138">String</span></span>|<span data-ttu-id="3b04d-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="3b04d-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="3b04d-140">description</span><span class="sxs-lookup"><span data-stu-id="3b04d-140">description</span></span>|<span data-ttu-id="3b04d-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b04d-141">String</span></span>|<span data-ttu-id="3b04d-142">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="3b04d-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="3b04d-143">permissions</span><span class="sxs-lookup"><span data-stu-id="3b04d-143">permissions</span></span>|<span data-ttu-id="3b04d-144">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3b04d-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3b04d-145">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="3b04d-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3b04d-146">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3b04d-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="3b04d-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="3b04d-147">rolePermissions</span></span>|<span data-ttu-id="3b04d-148">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3b04d-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="3b04d-149">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="3b04d-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="3b04d-150">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="3b04d-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="3b04d-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3b04d-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="3b04d-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b04d-152">Boolean</span></span>|<span data-ttu-id="3b04d-153">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="3b04d-153">Type of Role.</span></span> <span data-ttu-id="3b04d-154">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="3b04d-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="3b04d-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="3b04d-155">isBuiltIn</span></span>|<span data-ttu-id="3b04d-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b04d-156">Boolean</span></span>|<span data-ttu-id="3b04d-157">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="3b04d-157">Type of Role.</span></span> <span data-ttu-id="3b04d-158">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="3b04d-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="3b04d-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b04d-159">Response</span></span>
<span data-ttu-id="3b04d-160">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b04d-160">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b04d-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b04d-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b04d-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b04d-162">Request</span></span>
<span data-ttu-id="3b04d-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b04d-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 1145

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
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="3b04d-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b04d-164">Response</span></span>
<span data-ttu-id="3b04d-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b04d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





