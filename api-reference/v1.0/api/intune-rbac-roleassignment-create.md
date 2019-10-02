---
title: Criar roleAssignment
description: Criar um novo objeto roleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 837c69f2bf23c662c86769b308eae205767ca453
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361816"
---
# <a name="create-roleassignment"></a><span data-ttu-id="d61fa-103">Criar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d61fa-103">Create roleAssignment</span></span>

> <span data-ttu-id="d61fa-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d61fa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d61fa-105">Criar um novo objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d61fa-105">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d61fa-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d61fa-106">Prerequisites</span></span>
<span data-ttu-id="d61fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d61fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d61fa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d61fa-109">Permission type</span></span>|<span data-ttu-id="d61fa-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d61fa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d61fa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d61fa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d61fa-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d61fa-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d61fa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d61fa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d61fa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d61fa-114">Not supported.</span></span>|
|<span data-ttu-id="d61fa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d61fa-115">Application</span></span>|<span data-ttu-id="d61fa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d61fa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d61fa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d61fa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="d61fa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d61fa-118">Request headers</span></span>
|<span data-ttu-id="d61fa-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d61fa-119">Header</span></span>|<span data-ttu-id="d61fa-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d61fa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d61fa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d61fa-121">Authorization</span></span>|<span data-ttu-id="d61fa-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d61fa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d61fa-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d61fa-123">Accept</span></span>|<span data-ttu-id="d61fa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d61fa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d61fa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d61fa-125">Request body</span></span>
<span data-ttu-id="d61fa-126">No corpo da solicitação, forneça uma representação JSON do objeto roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="d61fa-126">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="d61fa-127">A tabela a seguir mostra as propriedades que são necessárias ao criar roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="d61fa-127">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="d61fa-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d61fa-128">Property</span></span>|<span data-ttu-id="d61fa-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d61fa-129">Type</span></span>|<span data-ttu-id="d61fa-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d61fa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d61fa-131">id</span><span class="sxs-lookup"><span data-stu-id="d61fa-131">id</span></span>|<span data-ttu-id="d61fa-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d61fa-132">String</span></span>|<span data-ttu-id="d61fa-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d61fa-133">Key of the entity.</span></span> <span data-ttu-id="d61fa-134">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d61fa-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="d61fa-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d61fa-135">displayName</span></span>|<span data-ttu-id="d61fa-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d61fa-136">String</span></span>|<span data-ttu-id="d61fa-137">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d61fa-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="d61fa-138">descrição</span><span class="sxs-lookup"><span data-stu-id="d61fa-138">description</span></span>|<span data-ttu-id="d61fa-139">String</span><span class="sxs-lookup"><span data-stu-id="d61fa-139">String</span></span>|<span data-ttu-id="d61fa-140">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d61fa-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="d61fa-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="d61fa-141">resourceScopes</span></span>|<span data-ttu-id="d61fa-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d61fa-142">String collection</span></span>|<span data-ttu-id="d61fa-143">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="d61fa-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="d61fa-144">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d61fa-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="d61fa-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d61fa-145">Response</span></span>
<span data-ttu-id="d61fa-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d61fa-146">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d61fa-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d61fa-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d61fa-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d61fa-148">Request</span></span>
<span data-ttu-id="d61fa-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d61fa-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d61fa-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d61fa-150">Response</span></span>
<span data-ttu-id="d61fa-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d61fa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




