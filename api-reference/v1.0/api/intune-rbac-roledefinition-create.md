---
title: Criar roleDefinition
description: Criar um novo objeto roleDefinition
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e331d5f11874408226cc946058001ad300f46dea
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752480"
---
# <a name="create-roledefinition"></a><span data-ttu-id="92a36-103">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="92a36-103">Create roleDefinition</span></span>

<span data-ttu-id="92a36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92a36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92a36-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92a36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92a36-106">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92a36-106">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92a36-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92a36-107">Prerequisites</span></span>
<span data-ttu-id="92a36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92a36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92a36-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92a36-110">Permission type</span></span>|<span data-ttu-id="92a36-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92a36-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92a36-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92a36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92a36-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92a36-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="92a36-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92a36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92a36-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92a36-115">Not supported.</span></span>|
|<span data-ttu-id="92a36-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92a36-116">Application</span></span>|<span data-ttu-id="92a36-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92a36-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92a36-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92a36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="92a36-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92a36-119">Request headers</span></span>
|<span data-ttu-id="92a36-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92a36-120">Header</span></span>|<span data-ttu-id="92a36-121">Valor</span><span class="sxs-lookup"><span data-stu-id="92a36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92a36-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="92a36-122">Authorization</span></span>|<span data-ttu-id="92a36-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92a36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92a36-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92a36-124">Accept</span></span>|<span data-ttu-id="92a36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92a36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92a36-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92a36-126">Request body</span></span>
<span data-ttu-id="92a36-127">No corpo da solicitação, forneça uma representação JSON do objeto roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="92a36-127">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="92a36-128">A tabela a seguir mostra as propriedades obrigatórias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="92a36-128">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="92a36-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92a36-129">Property</span></span>|<span data-ttu-id="92a36-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="92a36-130">Type</span></span>|<span data-ttu-id="92a36-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="92a36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92a36-132">id</span><span class="sxs-lookup"><span data-stu-id="92a36-132">id</span></span>|<span data-ttu-id="92a36-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92a36-133">String</span></span>|<span data-ttu-id="92a36-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="92a36-134">Key of the entity.</span></span> <span data-ttu-id="92a36-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="92a36-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="92a36-136">displayName</span><span class="sxs-lookup"><span data-stu-id="92a36-136">displayName</span></span>|<span data-ttu-id="92a36-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92a36-137">String</span></span>|<span data-ttu-id="92a36-138">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="92a36-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="92a36-139">descrição</span><span class="sxs-lookup"><span data-stu-id="92a36-139">description</span></span>|<span data-ttu-id="92a36-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92a36-140">String</span></span>|<span data-ttu-id="92a36-141">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="92a36-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="92a36-142">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="92a36-142">rolePermissions</span></span>|<span data-ttu-id="92a36-143">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="92a36-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="92a36-144">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="92a36-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="92a36-145">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="92a36-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="92a36-146">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="92a36-146">isBuiltIn</span></span>|<span data-ttu-id="92a36-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="92a36-147">Boolean</span></span>|<span data-ttu-id="92a36-148">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="92a36-148">Type of Role.</span></span> <span data-ttu-id="92a36-149">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="92a36-149">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="92a36-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="92a36-150">Response</span></span>
<span data-ttu-id="92a36-151">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92a36-151">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92a36-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92a36-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="92a36-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92a36-153">Request</span></span>
<span data-ttu-id="92a36-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92a36-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="92a36-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="92a36-155">Response</span></span>
<span data-ttu-id="92a36-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92a36-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




