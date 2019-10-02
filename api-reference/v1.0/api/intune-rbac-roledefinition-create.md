---
title: Criar roleDefinition
description: Criar um novo objeto roleDefinition
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 947033aabd05459995965c66bd0c83a0606f0eda
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361746"
---
# <a name="create-roledefinition"></a><span data-ttu-id="916ec-103">Criar roleDefinition</span><span class="sxs-lookup"><span data-stu-id="916ec-103">Create roleDefinition</span></span>

> <span data-ttu-id="916ec-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="916ec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="916ec-105">Criar um novo objeto [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="916ec-105">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="916ec-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="916ec-106">Prerequisites</span></span>
<span data-ttu-id="916ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="916ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="916ec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="916ec-109">Permission type</span></span>|<span data-ttu-id="916ec-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="916ec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="916ec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="916ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="916ec-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="916ec-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="916ec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="916ec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="916ec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="916ec-114">Not supported.</span></span>|
|<span data-ttu-id="916ec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="916ec-115">Application</span></span>|<span data-ttu-id="916ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="916ec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="916ec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="916ec-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="916ec-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="916ec-118">Request headers</span></span>
|<span data-ttu-id="916ec-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="916ec-119">Header</span></span>|<span data-ttu-id="916ec-120">Valor</span><span class="sxs-lookup"><span data-stu-id="916ec-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="916ec-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="916ec-121">Authorization</span></span>|<span data-ttu-id="916ec-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="916ec-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="916ec-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="916ec-123">Accept</span></span>|<span data-ttu-id="916ec-124">application/json</span><span class="sxs-lookup"><span data-stu-id="916ec-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="916ec-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="916ec-125">Request body</span></span>
<span data-ttu-id="916ec-126">No corpo da solicitação, forneça uma representação JSON do objeto roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="916ec-126">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="916ec-127">A tabela a seguir mostra as propriedades obrigatórias ao criar roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="916ec-127">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="916ec-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="916ec-128">Property</span></span>|<span data-ttu-id="916ec-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="916ec-129">Type</span></span>|<span data-ttu-id="916ec-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="916ec-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="916ec-131">id</span><span class="sxs-lookup"><span data-stu-id="916ec-131">id</span></span>|<span data-ttu-id="916ec-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="916ec-132">String</span></span>|<span data-ttu-id="916ec-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="916ec-133">Key of the entity.</span></span> <span data-ttu-id="916ec-134">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="916ec-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="916ec-135">displayName</span><span class="sxs-lookup"><span data-stu-id="916ec-135">displayName</span></span>|<span data-ttu-id="916ec-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="916ec-136">String</span></span>|<span data-ttu-id="916ec-137">Nome de exibição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="916ec-137">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="916ec-138">descrição</span><span class="sxs-lookup"><span data-stu-id="916ec-138">description</span></span>|<span data-ttu-id="916ec-139">String</span><span class="sxs-lookup"><span data-stu-id="916ec-139">String</span></span>|<span data-ttu-id="916ec-140">Descrição da definição de Função.</span><span class="sxs-lookup"><span data-stu-id="916ec-140">Description of the Role definition.</span></span>|
|<span data-ttu-id="916ec-141">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="916ec-141">rolePermissions</span></span>|<span data-ttu-id="916ec-142">Coleção [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="916ec-142">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="916ec-143">Lista de Permissões de Função que esta função está autorizada a executar.</span><span class="sxs-lookup"><span data-stu-id="916ec-143">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="916ec-144">Elas devem corresponder ao actionName definido como parte de rolePermission.</span><span class="sxs-lookup"><span data-stu-id="916ec-144">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="916ec-145">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="916ec-145">isBuiltIn</span></span>|<span data-ttu-id="916ec-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="916ec-146">Boolean</span></span>|<span data-ttu-id="916ec-147">Tipo de Função.</span><span class="sxs-lookup"><span data-stu-id="916ec-147">Type of Role.</span></span> <span data-ttu-id="916ec-148">Defina como True se for uma definição de função interna ou como False se for uma definição de função personalizada.</span><span class="sxs-lookup"><span data-stu-id="916ec-148">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="916ec-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="916ec-149">Response</span></span>
<span data-ttu-id="916ec-150">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [roleDefinition](../resources/intune-rbac-roledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="916ec-150">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="916ec-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="916ec-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="916ec-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="916ec-152">Request</span></span>
<span data-ttu-id="916ec-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="916ec-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="916ec-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="916ec-154">Response</span></span>
<span data-ttu-id="916ec-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="916ec-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




