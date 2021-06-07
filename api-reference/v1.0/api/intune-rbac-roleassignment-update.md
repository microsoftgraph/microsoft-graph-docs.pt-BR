---
title: Atualizar roleAssignment
description: Atualizar as propriedades de um objeto roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6550f0fa4f054c821482f0af00d19fc2d519263e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756818"
---
# <a name="update-roleassignment"></a><span data-ttu-id="6cd47-103">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="6cd47-103">Update roleAssignment</span></span>

<span data-ttu-id="6cd47-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cd47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cd47-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6cd47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cd47-106">Atualizar as propriedades de um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6cd47-106">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cd47-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6cd47-107">Prerequisites</span></span>
<span data-ttu-id="6cd47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cd47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cd47-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cd47-110">Permission type</span></span>|<span data-ttu-id="6cd47-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6cd47-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cd47-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cd47-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6cd47-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd47-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="6cd47-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cd47-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cd47-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cd47-115">Not supported.</span></span>|
|<span data-ttu-id="6cd47-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cd47-116">Application</span></span>|<span data-ttu-id="6cd47-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd47-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cd47-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cd47-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6cd47-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cd47-119">Request headers</span></span>
|<span data-ttu-id="6cd47-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cd47-120">Header</span></span>|<span data-ttu-id="6cd47-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6cd47-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cd47-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cd47-122">Authorization</span></span>|<span data-ttu-id="6cd47-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cd47-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cd47-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6cd47-124">Accept</span></span>|<span data-ttu-id="6cd47-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6cd47-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cd47-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cd47-126">Request body</span></span>
<span data-ttu-id="6cd47-127">No corpo da solicitação, forneça uma representação JSON do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6cd47-127">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="6cd47-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6cd47-128">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="6cd47-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cd47-129">Property</span></span>|<span data-ttu-id="6cd47-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cd47-130">Type</span></span>|<span data-ttu-id="6cd47-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cd47-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cd47-132">id</span><span class="sxs-lookup"><span data-stu-id="6cd47-132">id</span></span>|<span data-ttu-id="6cd47-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cd47-133">String</span></span>|<span data-ttu-id="6cd47-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6cd47-134">Key of the entity.</span></span> <span data-ttu-id="6cd47-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="6cd47-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="6cd47-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6cd47-136">displayName</span></span>|<span data-ttu-id="6cd47-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cd47-137">String</span></span>|<span data-ttu-id="6cd47-138">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="6cd47-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="6cd47-139">descrição</span><span class="sxs-lookup"><span data-stu-id="6cd47-139">description</span></span>|<span data-ttu-id="6cd47-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cd47-140">String</span></span>|<span data-ttu-id="6cd47-141">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="6cd47-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="6cd47-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="6cd47-142">resourceScopes</span></span>|<span data-ttu-id="6cd47-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cd47-143">String collection</span></span>|<span data-ttu-id="6cd47-144">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="6cd47-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="6cd47-145">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6cd47-145">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="6cd47-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cd47-146">Response</span></span>
<span data-ttu-id="6cd47-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cd47-147">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cd47-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cd47-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cd47-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cd47-149">Request</span></span>
<span data-ttu-id="6cd47-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cd47-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
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

### <a name="response"></a><span data-ttu-id="6cd47-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cd47-151">Response</span></span>
<span data-ttu-id="6cd47-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cd47-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




