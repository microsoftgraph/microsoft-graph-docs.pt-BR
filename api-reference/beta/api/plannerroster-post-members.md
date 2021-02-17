---
title: Criar plannerRosterMember
description: Crie um novo objeto plannerRosterMember.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: e7dac57941d50ee8b543c53982c216c4c19d5d07
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272420"
---
# <a name="create-plannerrostermember"></a><span data-ttu-id="234de-103">Criar plannerRosterMember</span><span class="sxs-lookup"><span data-stu-id="234de-103">Create plannerRosterMember</span></span>
<span data-ttu-id="234de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="234de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="234de-105">Adicione um membro ao [objeto plannerRoster.](../resources/plannerrostermember.md)</span><span class="sxs-lookup"><span data-stu-id="234de-105">Add a member to the [plannerRoster](../resources/plannerrostermember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="234de-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="234de-106">Permissions</span></span>
<span data-ttu-id="234de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="234de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="234de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="234de-109">Permission type</span></span>|<span data-ttu-id="234de-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="234de-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="234de-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="234de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="234de-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="234de-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="234de-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="234de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="234de-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="234de-114">Not supported.</span></span>|
|<span data-ttu-id="234de-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="234de-115">Application</span></span>|<span data-ttu-id="234de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="234de-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="234de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="234de-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /planner/rosters/{plannerRosterId}/members
```

## <a name="request-headers"></a><span data-ttu-id="234de-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="234de-118">Request headers</span></span>
|<span data-ttu-id="234de-119">Nome</span><span class="sxs-lookup"><span data-stu-id="234de-119">Name</span></span>|<span data-ttu-id="234de-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="234de-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="234de-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="234de-121">Authorization</span></span>|<span data-ttu-id="234de-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="234de-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="234de-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="234de-124">Content-Type</span></span>|<span data-ttu-id="234de-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="234de-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="234de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="234de-127">Request body</span></span>
<span data-ttu-id="234de-128">No corpo da solicitação, fornece uma representação JSON do objeto [plannerRosterMember.](../resources/plannerrostermember.md)</span><span class="sxs-lookup"><span data-stu-id="234de-128">In the request body, supply a JSON representation of the [plannerRosterMember](../resources/plannerrostermember.md) object.</span></span>

<span data-ttu-id="234de-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [plannerRosterMember](../resources/plannerrostermember.md).</span><span class="sxs-lookup"><span data-stu-id="234de-129">The following table shows the properties that are required when you create the [plannerRosterMember](../resources/plannerrostermember.md).</span></span>

|<span data-ttu-id="234de-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="234de-130">Property</span></span>|<span data-ttu-id="234de-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="234de-131">Type</span></span>|<span data-ttu-id="234de-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="234de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="234de-133">userId</span><span class="sxs-lookup"><span data-stu-id="234de-133">userId</span></span>|<span data-ttu-id="234de-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="234de-134">String</span></span>|<span data-ttu-id="234de-135">Identificador do .</span><span class="sxs-lookup"><span data-stu-id="234de-135">Identifier of the .</span></span>|
|<span data-ttu-id="234de-136">tenantId</span><span class="sxs-lookup"><span data-stu-id="234de-136">tenantId</span></span>|<span data-ttu-id="234de-137">String</span><span class="sxs-lookup"><span data-stu-id="234de-137">String</span></span>|<span data-ttu-id="234de-138">Identificador do locatário ao que o usuário pertence.</span><span class="sxs-lookup"><span data-stu-id="234de-138">Identifier of the tenant the user belongs to.</span></span> <span data-ttu-id="234de-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="234de-139">Optional.</span></span> <span data-ttu-id="234de-140">Atualmente, os membros da lista de participantes não podem ser de locatários diferentes.</span><span class="sxs-lookup"><span data-stu-id="234de-140">Currently roster members cannot be from different tenants.</span></span>|
|<span data-ttu-id="234de-141">funções</span><span class="sxs-lookup"><span data-stu-id="234de-141">roles</span></span>|<span data-ttu-id="234de-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="234de-142">String collection</span></span>|<span data-ttu-id="234de-143">Funções adicionais atribuídas ao usuário.</span><span class="sxs-lookup"><span data-stu-id="234de-143">Additional roles assigned to the user.</span></span> <span data-ttu-id="234de-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="234de-144">Optional.</span></span> <span data-ttu-id="234de-145">Atualmente, não há funções adicionais disponíveis para os usuários.</span><span class="sxs-lookup"><span data-stu-id="234de-145">Currently there are no additional roles available for users.</span></span>|



## <a name="response"></a><span data-ttu-id="234de-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="234de-146">Response</span></span>

<span data-ttu-id="234de-147">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [plannerRosterMember](../resources/plannerrostermember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="234de-147">If successful, this method returns a `201 Created` response code and a [plannerRosterMember](../resources/plannerrostermember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="234de-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="234de-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="234de-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="234de-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="234de-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="234de-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerrostermember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members
Content-Type: application/json
Content-length: 78

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "userId": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="234de-151">C#</span><span class="sxs-lookup"><span data-stu-id="234de-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerrostermember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="234de-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="234de-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerrostermember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="234de-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="234de-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerrostermember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="234de-154">Java</span><span class="sxs-lookup"><span data-stu-id="234de-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-plannerrostermember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="234de-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="234de-155">Response</span></span>
<span data-ttu-id="234de-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="234de-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRosterMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "id": "670095cd-95cd-6700-cd95-0067cd950067",
  "userId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
  "roles": [
  ]
}
```

