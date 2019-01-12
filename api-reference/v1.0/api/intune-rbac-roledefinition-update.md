---
title: Atualizar roleDefinition
description: Atualizar as propriedades de um objeto roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 37161711cf2803150c07da4fce010aec6893bf63
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946746"
---
# <a name="update-roledefinition"></a><span data-ttu-id="c4251-103">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="c4251-103">Update roleDefinition</span></span>

> <span data-ttu-id="c4251-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c4251-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4251-105">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c4251-105">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c4251-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4251-106">Prerequisites</span></span>
<span data-ttu-id="c4251-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4251-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4251-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4251-109">Permission type</span></span>|<span data-ttu-id="c4251-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4251-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4251-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4251-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c4251-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4251-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c4251-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4251-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4251-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4251-114">Not supported.</span></span>|
|<span data-ttu-id="c4251-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4251-115">Application</span></span>|<span data-ttu-id="c4251-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4251-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4251-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4251-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="c4251-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4251-118">Request headers</span></span>
|<span data-ttu-id="c4251-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4251-119">Header</span></span>|<span data-ttu-id="c4251-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c4251-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4251-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4251-121">Authorization</span></span>|<span data-ttu-id="c4251-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4251-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4251-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4251-123">Accept</span></span>|<span data-ttu-id="c4251-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c4251-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4251-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4251-125">Request body</span></span>
<span data-ttu-id="c4251-126">No corpo da solicitação, forneça uma representação JSON do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c4251-126">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="c4251-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c4251-127">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="c4251-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4251-128">Property</span></span>|<span data-ttu-id="c4251-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4251-129">Type</span></span>|<span data-ttu-id="c4251-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4251-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4251-131">id</span><span class="sxs-lookup"><span data-stu-id="c4251-131">id</span></span>|<span data-ttu-id="c4251-132">String</span><span class="sxs-lookup"><span data-stu-id="c4251-132">String</span></span>|<span data-ttu-id="c4251-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c4251-133">Key of the entity.</span></span> <span data-ttu-id="c4251-134">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c4251-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="c4251-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c4251-135">displayName</span></span>|<span data-ttu-id="c4251-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4251-136">String</span></span>|<span data-ttu-id="c4251-137">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="c4251-137">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="c4251-138">description</span><span class="sxs-lookup"><span data-stu-id="c4251-138">description</span></span>|<span data-ttu-id="c4251-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4251-139">String</span></span>|<span data-ttu-id="c4251-140">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="c4251-140">Description of the Role definition.</span></span>|
|<span data-ttu-id="c4251-141">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="c4251-141">rolePermissions</span></span>|<span data-ttu-id="c4251-142">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="c4251-142">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c4251-143">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="c4251-143">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c4251-144">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="c4251-144">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="c4251-145">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="c4251-145">isBuiltIn</span></span>|<span data-ttu-id="c4251-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4251-146">Boolean</span></span>|<span data-ttu-id="c4251-147">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="c4251-147">Type of Role.</span></span> <span data-ttu-id="c4251-148">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="c4251-148">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="c4251-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4251-149">Response</span></span>
<span data-ttu-id="c4251-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4251-150">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4251-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4251-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="c4251-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4251-152">Request</span></span>
<span data-ttu-id="c4251-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4251-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 580

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="c4251-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4251-154">Response</span></span>
<span data-ttu-id="c4251-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4251-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 629

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```



