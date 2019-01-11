---
title: Atualizar roleAssignment
description: Atualizar as propriedades de um objeto roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: edcfa7d06cbe4348835109c2adc3a48d9f24fe7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816209"
---
# <a name="update-roleassignment"></a><span data-ttu-id="8a18c-103">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="8a18c-103">Update roleAssignment</span></span>

> <span data-ttu-id="8a18c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8a18c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a18c-105">Atualizar as propriedades de um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8a18c-105">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a18c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a18c-106">Prerequisites</span></span>
<span data-ttu-id="8a18c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a18c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a18c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a18c-109">Permission type</span></span>|<span data-ttu-id="8a18c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a18c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a18c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a18c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8a18c-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a18c-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8a18c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a18c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a18c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a18c-114">Not supported.</span></span>|
|<span data-ttu-id="8a18c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a18c-115">Application</span></span>|<span data-ttu-id="8a18c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a18c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a18c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a18c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8a18c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a18c-118">Request headers</span></span>
|<span data-ttu-id="8a18c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a18c-119">Header</span></span>|<span data-ttu-id="8a18c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8a18c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a18c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a18c-121">Authorization</span></span>|<span data-ttu-id="8a18c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a18c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a18c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a18c-123">Accept</span></span>|<span data-ttu-id="8a18c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8a18c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a18c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a18c-125">Request body</span></span>
<span data-ttu-id="8a18c-126">No corpo da solicitação, forneça uma representação JSON do objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8a18c-126">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="8a18c-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8a18c-127">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="8a18c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a18c-128">Property</span></span>|<span data-ttu-id="8a18c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a18c-129">Type</span></span>|<span data-ttu-id="8a18c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a18c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a18c-131">id</span><span class="sxs-lookup"><span data-stu-id="8a18c-131">id</span></span>|<span data-ttu-id="8a18c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a18c-132">String</span></span>|<span data-ttu-id="8a18c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8a18c-133">Key of the entity.</span></span> <span data-ttu-id="8a18c-134">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="8a18c-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="8a18c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8a18c-135">displayName</span></span>|<span data-ttu-id="8a18c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a18c-136">String</span></span>|<span data-ttu-id="8a18c-137">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="8a18c-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="8a18c-138">descrição</span><span class="sxs-lookup"><span data-stu-id="8a18c-138">description</span></span>|<span data-ttu-id="8a18c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a18c-139">String</span></span>|<span data-ttu-id="8a18c-140">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="8a18c-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="8a18c-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="8a18c-141">resourceScopes</span></span>|<span data-ttu-id="8a18c-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a18c-142">String collection</span></span>|<span data-ttu-id="8a18c-143">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="8a18c-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="8a18c-144">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8a18c-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="8a18c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a18c-145">Response</span></span>
<span data-ttu-id="8a18c-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a18c-146">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a18c-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a18c-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a18c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a18c-148">Request</span></span>
<span data-ttu-id="8a18c-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a18c-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a18c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a18c-150">Response</span></span>
<span data-ttu-id="8a18c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a18c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



