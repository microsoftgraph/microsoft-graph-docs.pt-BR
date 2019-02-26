---
title: Criar deviceAndAppManagementRoleDefinition
description: Cria um novo objeto deviceAndAppManagementRoleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e622d2e201922e015dd38bf32d37e2693255fe14
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256522"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="f10ad-103">Criar deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f10ad-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="f10ad-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f10ad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f10ad-105">Cria um novo objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="f10ad-105">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f10ad-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f10ad-106">Prerequisites</span></span>
<span data-ttu-id="f10ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f10ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f10ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f10ad-109">Permission type</span></span>|<span data-ttu-id="f10ad-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f10ad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f10ad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f10ad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f10ad-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f10ad-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f10ad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f10ad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f10ad-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f10ad-114">Not supported.</span></span>|
|<span data-ttu-id="f10ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f10ad-115">Application</span></span>|<span data-ttu-id="f10ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f10ad-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f10ad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f10ad-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="f10ad-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f10ad-118">Request headers</span></span>
|<span data-ttu-id="f10ad-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f10ad-119">Header</span></span>|<span data-ttu-id="f10ad-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f10ad-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f10ad-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f10ad-121">Authorization</span></span>|<span data-ttu-id="f10ad-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f10ad-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f10ad-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f10ad-123">Accept</span></span>|<span data-ttu-id="f10ad-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f10ad-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f10ad-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f10ad-125">Request body</span></span>
<span data-ttu-id="f10ad-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="f10ad-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="f10ad-127">A tabela a seguir mostra as propriedades obrigatórias ao criar deviceAndAppManagementRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="f10ad-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="f10ad-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f10ad-128">Property</span></span>|<span data-ttu-id="f10ad-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f10ad-129">Type</span></span>|<span data-ttu-id="f10ad-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f10ad-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f10ad-131">id</span><span class="sxs-lookup"><span data-stu-id="f10ad-131">id</span></span>|<span data-ttu-id="f10ad-132">String</span><span class="sxs-lookup"><span data-stu-id="f10ad-132">String</span></span>|<span data-ttu-id="f10ad-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f10ad-133">Key of the entity.</span></span> <span data-ttu-id="f10ad-134">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="f10ad-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="f10ad-135">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f10ad-135">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f10ad-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f10ad-136">displayName</span></span>|<span data-ttu-id="f10ad-137">String</span><span class="sxs-lookup"><span data-stu-id="f10ad-137">String</span></span>|<span data-ttu-id="f10ad-138">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="f10ad-138">Display Name of the Role definition.</span></span> <span data-ttu-id="f10ad-139">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f10ad-139">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f10ad-140">description</span><span class="sxs-lookup"><span data-stu-id="f10ad-140">description</span></span>|<span data-ttu-id="f10ad-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f10ad-141">String</span></span>|<span data-ttu-id="f10ad-142">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="f10ad-142">Description of the Role definition.</span></span> <span data-ttu-id="f10ad-143">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f10ad-143">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f10ad-144">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="f10ad-144">rolePermissions</span></span>|<span data-ttu-id="f10ad-145">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f10ad-145">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="f10ad-146">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="f10ad-146">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="f10ad-147">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="f10ad-147">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="f10ad-148">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f10ad-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f10ad-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="f10ad-149">isBuiltIn</span></span>|<span data-ttu-id="f10ad-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="f10ad-150">Boolean</span></span>|<span data-ttu-id="f10ad-151">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="f10ad-151">Type of Role.</span></span> <span data-ttu-id="f10ad-152">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="f10ad-152">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="f10ad-153">Herdado de [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f10ad-153">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f10ad-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f10ad-154">Response</span></span>
<span data-ttu-id="f10ad-155">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f10ad-155">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f10ad-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f10ad-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="f10ad-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f10ad-157">Request</span></span>
<span data-ttu-id="f10ad-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f10ad-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f10ad-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f10ad-159">Response</span></span>
<span data-ttu-id="f10ad-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f10ad-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



