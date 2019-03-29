---
title: Atualizar deviceAndAppManagementRoleDefinition
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfcc2f315f528588739a780ea7f70b0207cab67d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961795"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="92324-103">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="92324-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="92324-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92324-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92324-105">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="92324-105">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92324-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92324-106">Prerequisites</span></span>
<span data-ttu-id="92324-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92324-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92324-109">Permission type</span></span>|<span data-ttu-id="92324-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92324-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92324-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92324-111">Delegated (work or school account)</span></span>|<span data-ttu-id="92324-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92324-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="92324-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92324-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92324-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92324-114">Not supported.</span></span>|
|<span data-ttu-id="92324-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92324-115">Application</span></span>|<span data-ttu-id="92324-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92324-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92324-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92324-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="92324-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92324-118">Request headers</span></span>
|<span data-ttu-id="92324-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92324-119">Header</span></span>|<span data-ttu-id="92324-120">Valor</span><span class="sxs-lookup"><span data-stu-id="92324-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92324-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="92324-121">Authorization</span></span>|<span data-ttu-id="92324-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92324-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92324-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92324-123">Accept</span></span>|<span data-ttu-id="92324-124">application/json</span><span class="sxs-lookup"><span data-stu-id="92324-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92324-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92324-125">Request body</span></span>
<span data-ttu-id="92324-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="92324-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="92324-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="92324-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="92324-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92324-128">Property</span></span>|<span data-ttu-id="92324-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="92324-129">Type</span></span>|<span data-ttu-id="92324-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="92324-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92324-131">id</span><span class="sxs-lookup"><span data-stu-id="92324-131">id</span></span>|<span data-ttu-id="92324-132">String</span><span class="sxs-lookup"><span data-stu-id="92324-132">String</span></span>|<span data-ttu-id="92324-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="92324-133">Key of the entity.</span></span> <span data-ttu-id="92324-134">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="92324-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="92324-135">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92324-135">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="92324-136">displayName</span><span class="sxs-lookup"><span data-stu-id="92324-136">displayName</span></span>|<span data-ttu-id="92324-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92324-137">String</span></span>|<span data-ttu-id="92324-138">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="92324-138">Display Name of the Role definition.</span></span> <span data-ttu-id="92324-139">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92324-139">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="92324-140">descrição</span><span class="sxs-lookup"><span data-stu-id="92324-140">description</span></span>|<span data-ttu-id="92324-141">String</span><span class="sxs-lookup"><span data-stu-id="92324-141">String</span></span>|<span data-ttu-id="92324-142">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="92324-142">Description of the Role definition.</span></span> <span data-ttu-id="92324-143">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92324-143">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="92324-144">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="92324-144">rolePermissions</span></span>|<span data-ttu-id="92324-145">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="92324-145">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="92324-146">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="92324-146">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="92324-147">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="92324-147">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="92324-148">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92324-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="92324-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="92324-149">isBuiltIn</span></span>|<span data-ttu-id="92324-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="92324-150">Boolean</span></span>|<span data-ttu-id="92324-151">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="92324-151">Type of Role.</span></span> <span data-ttu-id="92324-152">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="92324-152">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="92324-153">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92324-153">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="92324-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="92324-154">Response</span></span>
<span data-ttu-id="92324-155">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92324-155">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92324-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92324-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="92324-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92324-157">Request</span></span>
<span data-ttu-id="92324-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92324-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
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

### <a name="response"></a><span data-ttu-id="92324-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="92324-159">Response</span></span>
<span data-ttu-id="92324-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92324-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
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



