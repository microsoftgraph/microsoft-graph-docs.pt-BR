---
title: Atualizar roleAssignment
description: Atualizar as propriedades de um objeto roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3cd839aac57e726d693c497a4f9dba7afeb27f8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585374"
---
# <a name="update-roleassignment"></a><span data-ttu-id="b1a25-103">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="b1a25-103">Update roleAssignment</span></span>

> <span data-ttu-id="b1a25-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1a25-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1a25-105">Atualizar as propriedades de um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b1a25-105">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1a25-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1a25-106">Prerequisites</span></span>
<span data-ttu-id="b1a25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1a25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1a25-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1a25-109">Permission type</span></span>|<span data-ttu-id="b1a25-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1a25-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1a25-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1a25-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1a25-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1a25-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b1a25-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1a25-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1a25-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1a25-114">Not supported.</span></span>|
|<span data-ttu-id="b1a25-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1a25-115">Application</span></span>|<span data-ttu-id="b1a25-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1a25-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1a25-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1a25-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b1a25-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1a25-118">Request headers</span></span>
|<span data-ttu-id="b1a25-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1a25-119">Header</span></span>|<span data-ttu-id="b1a25-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b1a25-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1a25-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1a25-121">Authorization</span></span>|<span data-ttu-id="b1a25-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1a25-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1a25-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1a25-123">Accept</span></span>|<span data-ttu-id="b1a25-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b1a25-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1a25-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1a25-125">Request body</span></span>
<span data-ttu-id="b1a25-126">No corpo da solicitação, forneça uma representação JSON do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b1a25-126">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="b1a25-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b1a25-127">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="b1a25-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1a25-128">Property</span></span>|<span data-ttu-id="b1a25-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1a25-129">Type</span></span>|<span data-ttu-id="b1a25-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1a25-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1a25-131">id</span><span class="sxs-lookup"><span data-stu-id="b1a25-131">id</span></span>|<span data-ttu-id="b1a25-132">String</span><span class="sxs-lookup"><span data-stu-id="b1a25-132">String</span></span>|<span data-ttu-id="b1a25-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b1a25-133">Key of the entity.</span></span> <span data-ttu-id="b1a25-134">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="b1a25-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b1a25-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b1a25-135">displayName</span></span>|<span data-ttu-id="b1a25-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1a25-136">String</span></span>|<span data-ttu-id="b1a25-137">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="b1a25-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="b1a25-138">description</span><span class="sxs-lookup"><span data-stu-id="b1a25-138">description</span></span>|<span data-ttu-id="b1a25-139">String</span><span class="sxs-lookup"><span data-stu-id="b1a25-139">String</span></span>|<span data-ttu-id="b1a25-140">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="b1a25-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="b1a25-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b1a25-141">resourceScopes</span></span>|<span data-ttu-id="b1a25-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1a25-142">String collection</span></span>|<span data-ttu-id="b1a25-143">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="b1a25-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b1a25-144">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b1a25-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b1a25-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1a25-145">Response</span></span>
<span data-ttu-id="b1a25-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1a25-146">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1a25-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1a25-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1a25-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1a25-148">Request</span></span>
<span data-ttu-id="b1a25-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1a25-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1a25-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1a25-150">Response</span></span>
<span data-ttu-id="b1a25-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1a25-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



