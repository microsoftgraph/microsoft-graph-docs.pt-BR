---
title: Criar deviceAndAppManagementRoleDefinition
description: Cria um novo objeto deviceAndAppManagementRoleDefinition.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 281c965de97876812510b04a5f131f1354720df8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512318"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="0b240-103">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0b240-103">Create deviceAndAppManagementRoleDefinition</span></span>

<span data-ttu-id="0b240-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b240-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b240-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b240-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b240-106">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0b240-106">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b240-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b240-107">Prerequisites</span></span>
<span data-ttu-id="0b240-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b240-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b240-110">Permission type</span></span>|<span data-ttu-id="0b240-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b240-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b240-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b240-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b240-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b240-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0b240-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b240-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b240-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b240-115">Not supported.</span></span>|
|<span data-ttu-id="0b240-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b240-116">Application</span></span>|<span data-ttu-id="0b240-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b240-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b240-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b240-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="0b240-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b240-119">Request headers</span></span>
|<span data-ttu-id="0b240-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b240-120">Header</span></span>|<span data-ttu-id="0b240-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0b240-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b240-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b240-122">Authorization</span></span>|<span data-ttu-id="0b240-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b240-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b240-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b240-124">Accept</span></span>|<span data-ttu-id="0b240-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b240-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b240-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b240-126">Request body</span></span>
<span data-ttu-id="0b240-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="0b240-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="0b240-128">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="0b240-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="0b240-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b240-129">Property</span></span>|<span data-ttu-id="0b240-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b240-130">Type</span></span>|<span data-ttu-id="0b240-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b240-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b240-132">id</span><span class="sxs-lookup"><span data-stu-id="0b240-132">id</span></span>|<span data-ttu-id="0b240-133">String</span><span class="sxs-lookup"><span data-stu-id="0b240-133">String</span></span>|<span data-ttu-id="0b240-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0b240-134">Key of the entity.</span></span> <span data-ttu-id="0b240-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="0b240-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="0b240-136">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0b240-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="0b240-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0b240-137">displayName</span></span>|<span data-ttu-id="0b240-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b240-138">String</span></span>|<span data-ttu-id="0b240-139">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="0b240-139">Display Name of the Role definition.</span></span> <span data-ttu-id="0b240-140">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0b240-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="0b240-141">description</span><span class="sxs-lookup"><span data-stu-id="0b240-141">description</span></span>|<span data-ttu-id="0b240-142">String</span><span class="sxs-lookup"><span data-stu-id="0b240-142">String</span></span>|<span data-ttu-id="0b240-143">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="0b240-143">Description of the Role definition.</span></span> <span data-ttu-id="0b240-144">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0b240-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="0b240-145">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="0b240-145">rolePermissions</span></span>|<span data-ttu-id="0b240-146">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="0b240-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="0b240-147">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="0b240-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="0b240-148">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="0b240-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="0b240-149">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0b240-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="0b240-150">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="0b240-150">isBuiltIn</span></span>|<span data-ttu-id="0b240-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b240-151">Boolean</span></span>|<span data-ttu-id="0b240-152">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="0b240-152">Type of Role.</span></span> <span data-ttu-id="0b240-153">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="0b240-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="0b240-154">Herdada de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0b240-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0b240-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b240-155">Response</span></span>
<span data-ttu-id="0b240-156">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b240-156">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b240-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b240-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b240-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b240-158">Request</span></span>
<span data-ttu-id="0b240-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b240-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b240-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b240-160">Response</span></span>
<span data-ttu-id="0b240-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b240-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




