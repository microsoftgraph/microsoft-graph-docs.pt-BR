---
title: Criar roleAssignment
description: Criar um novo objeto roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b8f757d8131b40912b6e02ca402bb2f5aa622fc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961557"
---
# <a name="create-roleassignment"></a><span data-ttu-id="d7061-103">Criar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d7061-103">Create roleAssignment</span></span>

> <span data-ttu-id="d7061-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7061-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7061-105">Criar um novo objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d7061-105">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7061-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7061-106">Prerequisites</span></span>
<span data-ttu-id="d7061-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7061-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7061-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7061-109">Permission type</span></span>|<span data-ttu-id="d7061-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7061-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7061-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7061-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d7061-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7061-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d7061-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7061-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7061-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7061-114">Not supported.</span></span>|
|<span data-ttu-id="d7061-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7061-115">Application</span></span>|<span data-ttu-id="d7061-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7061-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7061-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7061-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="d7061-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7061-118">Request headers</span></span>
|<span data-ttu-id="d7061-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7061-119">Header</span></span>|<span data-ttu-id="d7061-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d7061-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7061-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7061-121">Authorization</span></span>|<span data-ttu-id="d7061-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7061-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7061-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7061-123">Accept</span></span>|<span data-ttu-id="d7061-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d7061-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7061-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7061-125">Request body</span></span>
<span data-ttu-id="d7061-126">No corpo da solicitação, forneça uma representação JSON do objeto roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="d7061-126">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="d7061-127">A tabela a seguir mostra as propriedades que são necessárias ao criar roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="d7061-127">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="d7061-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7061-128">Property</span></span>|<span data-ttu-id="d7061-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7061-129">Type</span></span>|<span data-ttu-id="d7061-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7061-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7061-131">id</span><span class="sxs-lookup"><span data-stu-id="d7061-131">id</span></span>|<span data-ttu-id="d7061-132">String</span><span class="sxs-lookup"><span data-stu-id="d7061-132">String</span></span>|<span data-ttu-id="d7061-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d7061-133">Key of the entity.</span></span> <span data-ttu-id="d7061-134">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d7061-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="d7061-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d7061-135">displayName</span></span>|<span data-ttu-id="d7061-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7061-136">String</span></span>|<span data-ttu-id="d7061-137">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d7061-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="d7061-138">descrição</span><span class="sxs-lookup"><span data-stu-id="d7061-138">description</span></span>|<span data-ttu-id="d7061-139">String</span><span class="sxs-lookup"><span data-stu-id="d7061-139">String</span></span>|<span data-ttu-id="d7061-140">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d7061-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="d7061-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="d7061-141">resourceScopes</span></span>|<span data-ttu-id="d7061-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7061-142">String collection</span></span>|<span data-ttu-id="d7061-143">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="d7061-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="d7061-144">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d7061-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="d7061-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7061-145">Response</span></span>
<span data-ttu-id="d7061-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7061-146">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7061-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7061-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7061-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7061-148">Request</span></span>
<span data-ttu-id="d7061-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7061-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d7061-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7061-150">Response</span></span>
<span data-ttu-id="d7061-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7061-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```



