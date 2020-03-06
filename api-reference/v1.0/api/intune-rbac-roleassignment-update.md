---
title: Atualizar roleAssignment
description: Atualizar as propriedades de um objeto roleAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06c71be971a4a3a37eed40568b3ec84d69d19b62
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512223"
---
# <a name="update-roleassignment"></a><span data-ttu-id="28067-103">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="28067-103">Update roleAssignment</span></span>

<span data-ttu-id="28067-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28067-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28067-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28067-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28067-106">Atualizar as propriedades de um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="28067-106">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28067-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28067-107">Prerequisites</span></span>
<span data-ttu-id="28067-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28067-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28067-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28067-110">Permission type</span></span>|<span data-ttu-id="28067-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="28067-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28067-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28067-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28067-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28067-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="28067-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28067-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28067-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28067-115">Not supported.</span></span>|
|<span data-ttu-id="28067-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28067-116">Application</span></span>|<span data-ttu-id="28067-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28067-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28067-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28067-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="28067-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28067-119">Request headers</span></span>
|<span data-ttu-id="28067-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28067-120">Header</span></span>|<span data-ttu-id="28067-121">Valor</span><span class="sxs-lookup"><span data-stu-id="28067-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28067-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="28067-122">Authorization</span></span>|<span data-ttu-id="28067-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28067-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28067-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="28067-124">Accept</span></span>|<span data-ttu-id="28067-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28067-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28067-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28067-126">Request body</span></span>
<span data-ttu-id="28067-127">No corpo da solicitação, forneça uma representação JSON do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="28067-127">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="28067-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="28067-128">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="28067-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28067-129">Property</span></span>|<span data-ttu-id="28067-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="28067-130">Type</span></span>|<span data-ttu-id="28067-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="28067-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28067-132">id</span><span class="sxs-lookup"><span data-stu-id="28067-132">id</span></span>|<span data-ttu-id="28067-133">String</span><span class="sxs-lookup"><span data-stu-id="28067-133">String</span></span>|<span data-ttu-id="28067-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="28067-134">Key of the entity.</span></span> <span data-ttu-id="28067-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="28067-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="28067-136">displayName</span><span class="sxs-lookup"><span data-stu-id="28067-136">displayName</span></span>|<span data-ttu-id="28067-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28067-137">String</span></span>|<span data-ttu-id="28067-138">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="28067-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="28067-139">description</span><span class="sxs-lookup"><span data-stu-id="28067-139">description</span></span>|<span data-ttu-id="28067-140">String</span><span class="sxs-lookup"><span data-stu-id="28067-140">String</span></span>|<span data-ttu-id="28067-141">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="28067-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="28067-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="28067-142">resourceScopes</span></span>|<span data-ttu-id="28067-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="28067-143">String collection</span></span>|<span data-ttu-id="28067-144">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="28067-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="28067-145">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="28067-145">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="28067-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="28067-146">Response</span></span>
<span data-ttu-id="28067-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28067-147">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28067-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28067-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="28067-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28067-149">Request</span></span>
<span data-ttu-id="28067-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28067-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="28067-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="28067-151">Response</span></span>
<span data-ttu-id="28067-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28067-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




