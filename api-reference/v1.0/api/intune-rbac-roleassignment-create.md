---
title: Criar roleAssignment
description: Criar um novo objeto roleAssignment.
author: tfitzmac
ms.openlocfilehash: ac3a8ee5b007c918a9b655cb2f396c872f9f2d92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362234"
---
# <a name="create-roleassignment"></a><span data-ttu-id="d4bf1-103">Criar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d4bf1-103">Create roleAssignment</span></span>

> <span data-ttu-id="d4bf1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4bf1-105">Criar um novo objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d4bf1-105">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4bf1-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4bf1-106">Prerequisites</span></span>
<span data-ttu-id="d4bf1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4bf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4bf1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4bf1-109">Permission type</span></span>|<span data-ttu-id="d4bf1-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4bf1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4bf1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4bf1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4bf1-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4bf1-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d4bf1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4bf1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4bf1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-114">Not supported.</span></span>|
|<span data-ttu-id="d4bf1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4bf1-115">Application</span></span>|<span data-ttu-id="d4bf1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4bf1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4bf1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="d4bf1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4bf1-118">Request headers</span></span>
|<span data-ttu-id="d4bf1-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4bf1-119">Header</span></span>|<span data-ttu-id="d4bf1-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d4bf1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4bf1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4bf1-121">Authorization</span></span>|<span data-ttu-id="d4bf1-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4bf1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d4bf1-123">Accept</span></span>|<span data-ttu-id="d4bf1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d4bf1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4bf1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4bf1-125">Request body</span></span>
<span data-ttu-id="d4bf1-126">No corpo da solicitação, forneça uma representação JSON do objeto roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-126">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="d4bf1-127">A tabela a seguir mostra as propriedades que são necessárias ao criar roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-127">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="d4bf1-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4bf1-128">Property</span></span>|<span data-ttu-id="d4bf1-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4bf1-129">Type</span></span>|<span data-ttu-id="d4bf1-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4bf1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4bf1-131">id</span><span class="sxs-lookup"><span data-stu-id="d4bf1-131">id</span></span>|<span data-ttu-id="d4bf1-132">String</span><span class="sxs-lookup"><span data-stu-id="d4bf1-132">String</span></span>|<span data-ttu-id="d4bf1-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-133">Key of the entity.</span></span> <span data-ttu-id="d4bf1-134">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="d4bf1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d4bf1-135">displayName</span></span>|<span data-ttu-id="d4bf1-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4bf1-136">String</span></span>|<span data-ttu-id="d4bf1-137">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="d4bf1-138">descrição</span><span class="sxs-lookup"><span data-stu-id="d4bf1-138">description</span></span>|<span data-ttu-id="d4bf1-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4bf1-139">String</span></span>|<span data-ttu-id="d4bf1-140">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="d4bf1-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="d4bf1-141">resourceScopes</span></span>|<span data-ttu-id="d4bf1-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4bf1-142">String collection</span></span>|<span data-ttu-id="d4bf1-143">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="d4bf1-144">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="d4bf1-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4bf1-145">Response</span></span>
<span data-ttu-id="d4bf1-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-146">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4bf1-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4bf1-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4bf1-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4bf1-148">Request</span></span>
<span data-ttu-id="d4bf1-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4bf1-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4bf1-150">Response</span></span>
<span data-ttu-id="d4bf1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4bf1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



