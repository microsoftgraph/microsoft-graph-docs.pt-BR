---
title: Criar deviceAndAppManagementRoleDefinition
description: Cria um novo objeto deviceAndAppManagementRoleDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3351d891e99699748a8792df343cc41e721eeb48
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069712"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="2864f-103">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="2864f-103">Create deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="2864f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2864f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2864f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2864f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2864f-106">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2864f-106">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2864f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2864f-107">Prerequisites</span></span>
<span data-ttu-id="2864f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2864f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2864f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2864f-110">Permission type</span></span>|<span data-ttu-id="2864f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2864f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2864f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2864f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2864f-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2864f-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="2864f-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2864f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2864f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2864f-115">Not supported.</span></span>|
|<span data-ttu-id="2864f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2864f-116">Application</span></span>|<span data-ttu-id="2864f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2864f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2864f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2864f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="2864f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2864f-119">Request headers</span></span>
|<span data-ttu-id="2864f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2864f-120">Header</span></span>|<span data-ttu-id="2864f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2864f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2864f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2864f-122">Authorization</span></span>|<span data-ttu-id="2864f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2864f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2864f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2864f-124">Accept</span></span>|<span data-ttu-id="2864f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2864f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2864f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2864f-126">Request body</span></span>
<span data-ttu-id="2864f-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="2864f-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="2864f-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="2864f-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="2864f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2864f-129">Property</span></span>|<span data-ttu-id="2864f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2864f-130">Type</span></span>|<span data-ttu-id="2864f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2864f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2864f-132">id</span><span class="sxs-lookup"><span data-stu-id="2864f-132">id</span></span>|<span data-ttu-id="2864f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2864f-133">String</span></span>|<span data-ttu-id="2864f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2864f-134">Key of the entity.</span></span> <span data-ttu-id="2864f-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="2864f-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="2864f-136">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2864f-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2864f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2864f-137">displayName</span></span>|<span data-ttu-id="2864f-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2864f-138">String</span></span>|<span data-ttu-id="2864f-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="2864f-139">Display Name of the Role definition.</span></span> <span data-ttu-id="2864f-140">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2864f-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2864f-141">description</span><span class="sxs-lookup"><span data-stu-id="2864f-141">description</span></span>|<span data-ttu-id="2864f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2864f-142">String</span></span>|<span data-ttu-id="2864f-143">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="2864f-143">Description of the Role definition.</span></span> <span data-ttu-id="2864f-144">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2864f-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2864f-145">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="2864f-145">rolePermissions</span></span>|<span data-ttu-id="2864f-146">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="2864f-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="2864f-147">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="2864f-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="2864f-148">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="2864f-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="2864f-149">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2864f-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="2864f-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="2864f-150">isBuiltIn</span></span>|<span data-ttu-id="2864f-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="2864f-151">Boolean</span></span>|<span data-ttu-id="2864f-152">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="2864f-152">Type of Role.</span></span> <span data-ttu-id="2864f-153">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="2864f-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="2864f-154">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="2864f-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2864f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="2864f-155">Response</span></span>
<span data-ttu-id="2864f-156">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2864f-156">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2864f-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2864f-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="2864f-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2864f-158">Request</span></span>
<span data-ttu-id="2864f-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2864f-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="2864f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="2864f-160">Response</span></span>
<span data-ttu-id="2864f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2864f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









