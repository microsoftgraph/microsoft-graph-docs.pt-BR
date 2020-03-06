---
title: Criar roleAssignment
description: Criar um novo objeto roleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34aca92a1d278f39d236865c4ac3484f0b5f10d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512240"
---
# <a name="create-roleassignment"></a><span data-ttu-id="bb096-103">Criar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="bb096-103">Create roleAssignment</span></span>

<span data-ttu-id="bb096-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb096-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb096-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb096-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb096-106">Criar um novo objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bb096-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb096-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb096-107">Prerequisites</span></span>
<span data-ttu-id="bb096-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb096-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb096-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb096-110">Permission type</span></span>|<span data-ttu-id="bb096-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb096-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb096-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb096-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb096-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb096-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="bb096-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb096-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb096-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb096-115">Not supported.</span></span>|
|<span data-ttu-id="bb096-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb096-116">Application</span></span>|<span data-ttu-id="bb096-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb096-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb096-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb096-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="bb096-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb096-119">Request headers</span></span>
|<span data-ttu-id="bb096-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb096-120">Header</span></span>|<span data-ttu-id="bb096-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bb096-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb096-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb096-122">Authorization</span></span>|<span data-ttu-id="bb096-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb096-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb096-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb096-124">Accept</span></span>|<span data-ttu-id="bb096-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb096-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb096-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb096-126">Request body</span></span>
<span data-ttu-id="bb096-127">No corpo da solicitação, forneça uma representação JSON do objeto roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="bb096-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="bb096-128">A tabela a seguir mostra as propriedades que são necessárias ao criar roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="bb096-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="bb096-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb096-129">Property</span></span>|<span data-ttu-id="bb096-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb096-130">Type</span></span>|<span data-ttu-id="bb096-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb096-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb096-132">id</span><span class="sxs-lookup"><span data-stu-id="bb096-132">id</span></span>|<span data-ttu-id="bb096-133">String</span><span class="sxs-lookup"><span data-stu-id="bb096-133">String</span></span>|<span data-ttu-id="bb096-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bb096-134">Key of the entity.</span></span> <span data-ttu-id="bb096-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="bb096-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="bb096-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bb096-136">displayName</span></span>|<span data-ttu-id="bb096-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb096-137">String</span></span>|<span data-ttu-id="bb096-138">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="bb096-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="bb096-139">description</span><span class="sxs-lookup"><span data-stu-id="bb096-139">description</span></span>|<span data-ttu-id="bb096-140">String</span><span class="sxs-lookup"><span data-stu-id="bb096-140">String</span></span>|<span data-ttu-id="bb096-141">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="bb096-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="bb096-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="bb096-142">resourceScopes</span></span>|<span data-ttu-id="bb096-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb096-143">String collection</span></span>|<span data-ttu-id="bb096-144">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="bb096-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="bb096-145">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bb096-145">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="bb096-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb096-146">Response</span></span>
<span data-ttu-id="bb096-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb096-147">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb096-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb096-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb096-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb096-149">Request</span></span>
<span data-ttu-id="bb096-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb096-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb096-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb096-151">Response</span></span>
<span data-ttu-id="bb096-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb096-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




