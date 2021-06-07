---
title: Atualizar deviceAndAppManagementRoleDefinition
description: Atualizar as propriedades de um objeto deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e7ad1fd0ad74df9e81ceeafc599e795a91f7f68c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756881"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="1f31a-103">Atualizar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1f31a-103">Update deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="1f31a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f31a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f31a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f31a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f31a-106">Atualizar as propriedades de um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="1f31a-106">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f31a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f31a-107">Prerequisites</span></span>
<span data-ttu-id="1f31a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f31a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f31a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f31a-110">Permission type</span></span>|<span data-ttu-id="1f31a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f31a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f31a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f31a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f31a-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f31a-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="1f31a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f31a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f31a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f31a-115">Not supported.</span></span>|
|<span data-ttu-id="1f31a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f31a-116">Application</span></span>|<span data-ttu-id="1f31a-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f31a-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f31a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f31a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="1f31a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f31a-119">Request headers</span></span>
|<span data-ttu-id="1f31a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f31a-120">Header</span></span>|<span data-ttu-id="1f31a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1f31a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f31a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f31a-122">Authorization</span></span>|<span data-ttu-id="1f31a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f31a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f31a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1f31a-124">Accept</span></span>|<span data-ttu-id="1f31a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f31a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f31a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f31a-126">Request body</span></span>
<span data-ttu-id="1f31a-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="1f31a-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="1f31a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="1f31a-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="1f31a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f31a-129">Property</span></span>|<span data-ttu-id="1f31a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f31a-130">Type</span></span>|<span data-ttu-id="1f31a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f31a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f31a-132">id</span><span class="sxs-lookup"><span data-stu-id="1f31a-132">id</span></span>|<span data-ttu-id="1f31a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f31a-133">String</span></span>|<span data-ttu-id="1f31a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1f31a-134">Key of the entity.</span></span> <span data-ttu-id="1f31a-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="1f31a-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="1f31a-136">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f31a-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="1f31a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1f31a-137">displayName</span></span>|<span data-ttu-id="1f31a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f31a-138">String</span></span>|<span data-ttu-id="1f31a-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="1f31a-139">Display Name of the Role definition.</span></span> <span data-ttu-id="1f31a-140">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f31a-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="1f31a-141">descrição</span><span class="sxs-lookup"><span data-stu-id="1f31a-141">description</span></span>|<span data-ttu-id="1f31a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f31a-142">String</span></span>|<span data-ttu-id="1f31a-143">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="1f31a-143">Description of the Role definition.</span></span> <span data-ttu-id="1f31a-144">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f31a-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="1f31a-145">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="1f31a-145">rolePermissions</span></span>|<span data-ttu-id="1f31a-146">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="1f31a-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="1f31a-147">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="1f31a-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="1f31a-148">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="1f31a-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="1f31a-149">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f31a-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="1f31a-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="1f31a-150">isBuiltIn</span></span>|<span data-ttu-id="1f31a-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="1f31a-151">Boolean</span></span>|<span data-ttu-id="1f31a-152">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="1f31a-152">Type of Role.</span></span> <span data-ttu-id="1f31a-153">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="1f31a-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="1f31a-154">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f31a-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1f31a-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f31a-155">Response</span></span>
<span data-ttu-id="1f31a-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f31a-156">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f31a-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f31a-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f31a-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f31a-158">Request</span></span>
<span data-ttu-id="1f31a-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f31a-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f31a-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f31a-160">Response</span></span>
<span data-ttu-id="1f31a-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f31a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




