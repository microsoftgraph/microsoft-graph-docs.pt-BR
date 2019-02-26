---
title: Atualizar roleDefinition
description: Atualizar as propriedades de um objeto roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdbc723059ee9134892569cb3a497de8b03cb016
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255000"
---
# <a name="update-roledefinition"></a><span data-ttu-id="463a4-103">Atualizar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="463a4-103">Update roleDefinition</span></span>

> <span data-ttu-id="463a4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="463a4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="463a4-105">Atualizar as propriedades de um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="463a4-105">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="463a4-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="463a4-106">Prerequisites</span></span>
<span data-ttu-id="463a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="463a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="463a4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="463a4-109">Permission type</span></span>|<span data-ttu-id="463a4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="463a4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="463a4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="463a4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="463a4-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="463a4-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="463a4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="463a4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="463a4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="463a4-114">Not supported.</span></span>|
|<span data-ttu-id="463a4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="463a4-115">Application</span></span>|<span data-ttu-id="463a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="463a4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="463a4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="463a4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="463a4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="463a4-118">Request headers</span></span>
|<span data-ttu-id="463a4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="463a4-119">Header</span></span>|<span data-ttu-id="463a4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="463a4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="463a4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="463a4-121">Authorization</span></span>|<span data-ttu-id="463a4-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="463a4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="463a4-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="463a4-123">Accept</span></span>|<span data-ttu-id="463a4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="463a4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="463a4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="463a4-125">Request body</span></span>
<span data-ttu-id="463a4-126">No corpo da solicitação, forneça uma representação JSON do objeto [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="463a4-126">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="463a4-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="463a4-127">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="463a4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="463a4-128">Property</span></span>|<span data-ttu-id="463a4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="463a4-129">Type</span></span>|<span data-ttu-id="463a4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="463a4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="463a4-131">id</span><span class="sxs-lookup"><span data-stu-id="463a4-131">id</span></span>|<span data-ttu-id="463a4-132">String</span><span class="sxs-lookup"><span data-stu-id="463a4-132">String</span></span>|<span data-ttu-id="463a4-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="463a4-133">Key of the entity.</span></span> <span data-ttu-id="463a4-134">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="463a4-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="463a4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="463a4-135">displayName</span></span>|<span data-ttu-id="463a4-136">String</span><span class="sxs-lookup"><span data-stu-id="463a4-136">String</span></span>|<span data-ttu-id="463a4-137">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="463a4-137">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="463a4-138">description</span><span class="sxs-lookup"><span data-stu-id="463a4-138">description</span></span>|<span data-ttu-id="463a4-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="463a4-139">String</span></span>|<span data-ttu-id="463a4-140">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="463a4-140">Description of the Role definition.</span></span>|
|<span data-ttu-id="463a4-141">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="463a4-141">rolePermissions</span></span>|<span data-ttu-id="463a4-142">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="463a4-142">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="463a4-143">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="463a4-143">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="463a4-144">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="463a4-144">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="463a4-145">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="463a4-145">isBuiltIn</span></span>|<span data-ttu-id="463a4-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="463a4-146">Boolean</span></span>|<span data-ttu-id="463a4-147">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="463a4-147">Type of Role.</span></span> <span data-ttu-id="463a4-148">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="463a4-148">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="463a4-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="463a4-149">Response</span></span>
<span data-ttu-id="463a4-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="463a4-150">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="463a4-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="463a4-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="463a4-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="463a4-152">Request</span></span>
<span data-ttu-id="463a4-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="463a4-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="463a4-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="463a4-154">Response</span></span>
<span data-ttu-id="463a4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="463a4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



