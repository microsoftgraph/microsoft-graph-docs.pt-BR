---
title: Criar roleAssignment
description: Criar um novo objeto roleAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6019357dcea7e020022eb5def2d449c9a5be47cd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456585"
---
# <a name="create-roleassignment"></a><span data-ttu-id="9adaf-103">Criar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="9adaf-103">Create roleAssignment</span></span>

<span data-ttu-id="9adaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9adaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9adaf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9adaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9adaf-106">Criar um novo objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9adaf-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9adaf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9adaf-107">Prerequisites</span></span>
<span data-ttu-id="9adaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9adaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9adaf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9adaf-110">Permission type</span></span>|<span data-ttu-id="9adaf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9adaf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9adaf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9adaf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9adaf-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9adaf-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="9adaf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9adaf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9adaf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9adaf-115">Not supported.</span></span>|
|<span data-ttu-id="9adaf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9adaf-116">Application</span></span>|<span data-ttu-id="9adaf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9adaf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9adaf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9adaf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="9adaf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9adaf-119">Request headers</span></span>
|<span data-ttu-id="9adaf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9adaf-120">Header</span></span>|<span data-ttu-id="9adaf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9adaf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9adaf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9adaf-122">Authorization</span></span>|<span data-ttu-id="9adaf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9adaf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9adaf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9adaf-124">Accept</span></span>|<span data-ttu-id="9adaf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9adaf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9adaf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9adaf-126">Request body</span></span>
<span data-ttu-id="9adaf-127">No corpo da solicitação, forneça uma representação JSON do objeto roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="9adaf-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="9adaf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="9adaf-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="9adaf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9adaf-129">Property</span></span>|<span data-ttu-id="9adaf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9adaf-130">Type</span></span>|<span data-ttu-id="9adaf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9adaf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9adaf-132">id</span><span class="sxs-lookup"><span data-stu-id="9adaf-132">id</span></span>|<span data-ttu-id="9adaf-133">String</span><span class="sxs-lookup"><span data-stu-id="9adaf-133">String</span></span>|<span data-ttu-id="9adaf-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9adaf-134">Key of the entity.</span></span> <span data-ttu-id="9adaf-135">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="9adaf-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="9adaf-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9adaf-136">displayName</span></span>|<span data-ttu-id="9adaf-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9adaf-137">String</span></span>|<span data-ttu-id="9adaf-138">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9adaf-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="9adaf-139">description</span><span class="sxs-lookup"><span data-stu-id="9adaf-139">description</span></span>|<span data-ttu-id="9adaf-140">String</span><span class="sxs-lookup"><span data-stu-id="9adaf-140">String</span></span>|<span data-ttu-id="9adaf-141">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9adaf-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="9adaf-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="9adaf-142">resourceScopes</span></span>|<span data-ttu-id="9adaf-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9adaf-143">String collection</span></span>|<span data-ttu-id="9adaf-144">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="9adaf-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="9adaf-145">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9adaf-145">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="9adaf-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9adaf-146">Response</span></span>
<span data-ttu-id="9adaf-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9adaf-147">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9adaf-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9adaf-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="9adaf-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9adaf-149">Request</span></span>
<span data-ttu-id="9adaf-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9adaf-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9adaf-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9adaf-151">Response</span></span>
<span data-ttu-id="9adaf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9adaf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






