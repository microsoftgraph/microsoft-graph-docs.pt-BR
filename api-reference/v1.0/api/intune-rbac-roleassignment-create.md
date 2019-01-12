---
title: Criar roleAssignment
description: Criar um novo objeto roleAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0cb60cad1785de83c44772d6f1cbc00c9129861f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973780"
---
# <a name="create-roleassignment"></a><span data-ttu-id="33237-103">Criar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="33237-103">Create roleAssignment</span></span>

> <span data-ttu-id="33237-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="33237-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33237-105">Criar um novo objeto [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="33237-105">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33237-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33237-106">Prerequisites</span></span>
<span data-ttu-id="33237-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33237-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33237-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33237-109">Permission type</span></span>|<span data-ttu-id="33237-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33237-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33237-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33237-111">Delegated (work or school account)</span></span>|<span data-ttu-id="33237-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33237-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="33237-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33237-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33237-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33237-114">Not supported.</span></span>|
|<span data-ttu-id="33237-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33237-115">Application</span></span>|<span data-ttu-id="33237-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33237-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33237-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33237-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="33237-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33237-118">Request headers</span></span>
|<span data-ttu-id="33237-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33237-119">Header</span></span>|<span data-ttu-id="33237-120">Valor</span><span class="sxs-lookup"><span data-stu-id="33237-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33237-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="33237-121">Authorization</span></span>|<span data-ttu-id="33237-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33237-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33237-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33237-123">Accept</span></span>|<span data-ttu-id="33237-124">application/json</span><span class="sxs-lookup"><span data-stu-id="33237-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33237-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33237-125">Request body</span></span>
<span data-ttu-id="33237-126">No corpo da solicitação, forneça uma representação JSON do objeto roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="33237-126">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="33237-127">A tabela a seguir mostra as propriedades que são necessárias ao criar roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="33237-127">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="33237-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33237-128">Property</span></span>|<span data-ttu-id="33237-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="33237-129">Type</span></span>|<span data-ttu-id="33237-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="33237-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33237-131">id</span><span class="sxs-lookup"><span data-stu-id="33237-131">id</span></span>|<span data-ttu-id="33237-132">String</span><span class="sxs-lookup"><span data-stu-id="33237-132">String</span></span>|<span data-ttu-id="33237-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="33237-133">Key of the entity.</span></span> <span data-ttu-id="33237-134">É somente leitura e é gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="33237-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="33237-135">displayName</span><span class="sxs-lookup"><span data-stu-id="33237-135">displayName</span></span>|<span data-ttu-id="33237-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33237-136">String</span></span>|<span data-ttu-id="33237-137">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="33237-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="33237-138">descrição</span><span class="sxs-lookup"><span data-stu-id="33237-138">description</span></span>|<span data-ttu-id="33237-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="33237-139">String</span></span>|<span data-ttu-id="33237-140">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="33237-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="33237-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="33237-141">resourceScopes</span></span>|<span data-ttu-id="33237-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="33237-142">String collection</span></span>|<span data-ttu-id="33237-143">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="33237-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="33237-144">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="33237-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="33237-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="33237-145">Response</span></span>
<span data-ttu-id="33237-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [roleAssignment](../resources/intune-rbac-roleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33237-146">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33237-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33237-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="33237-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33237-148">Request</span></span>
<span data-ttu-id="33237-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33237-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="33237-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="33237-150">Response</span></span>
<span data-ttu-id="33237-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33237-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



