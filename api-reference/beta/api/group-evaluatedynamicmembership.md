---
title: 'Grupo: evaluateDynamicMembership'
description: Avaliar se um usuário ou dispositivo é ou seria um membro de um grupo dinâmico.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a9dffefdc8a7f967cd44d16168ad83c822bacc69
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965317"
---
# <a name="group-evaluatedynamicmembership"></a><span data-ttu-id="8a8c4-103">Grupo: evaluateDynamicMembership</span><span class="sxs-lookup"><span data-stu-id="8a8c4-103">group: evaluateDynamicMembership</span></span>

<span data-ttu-id="8a8c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a8c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a8c4-105">Avaliar se um usuário ou dispositivo é ou seria membro de um grupo dinâmico.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-105">Evaluate whether a user or device is or would be a member of a dynamic group.</span></span> <span data-ttu-id="8a8c4-106">A regra de associação é retornada junto com outros detalhes que foram usados na avaliação.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-106">The membership rule is returned along with other details that were used in the evaluation.</span></span> <span data-ttu-id="8a8c4-107">Você pode concluir essa operação das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="8a8c4-107">You can complete this operation in the following ways:</span></span> 

- <span data-ttu-id="8a8c4-108">Avaliar se um usuário ou dispositivo é um membro de um grupo dinâmico especificado.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-108">Evaluate whether a user or device is a member of a specified dynamic group.</span></span>  
- <span data-ttu-id="8a8c4-109">Avaliar se um usuário ou dispositivo seria um membro de um grupo dinâmico com base na ID do usuário ou no dispositivo e em uma regra de associação.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-109">Evaluate whether a user or device would be a member of a dynamic group based on the ID of the user or device and a membership rule.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a8c4-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a8c4-110">Permissions</span></span>

<span data-ttu-id="8a8c4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a8c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a><span data-ttu-id="8a8c4-113">Avaliar associação dinâmica com ID de membro e ID de grupo</span><span class="sxs-lookup"><span data-stu-id="8a8c4-113">Evaluate dynamic membership with member ID and group ID</span></span>

| <span data-ttu-id="8a8c4-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a8c4-114">Permission type</span></span> | <span data-ttu-id="8a8c4-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a8c4-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="8a8c4-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a8c4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8a8c4-117">Para User: Group. Read. All e User. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="8a8c4-117">For user: Group.Read.All and User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="8a8c4-118">Para Device: Group. Read. All e Device. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="8a8c4-118">For device: Group.Read.All and Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="8a8c4-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a8c4-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a8c4-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-120">Not supported.</span></span> |
| <span data-ttu-id="8a8c4-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a8c4-121">Application</span></span>                            | <span data-ttu-id="8a8c4-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-122">Not supported.</span></span> |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a><span data-ttu-id="8a8c4-123">Avaliar associação dinâmica com ID de membro e regra de associação</span><span class="sxs-lookup"><span data-stu-id="8a8c4-123">Evaluate dynamic membership with member ID and membership rule</span></span>

| <span data-ttu-id="8a8c4-124">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a8c4-124">Permission type</span></span> | <span data-ttu-id="8a8c4-125">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a8c4-125">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="8a8c4-126">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a8c4-126">Delegated (work or school account)</span></span> | <span data-ttu-id="8a8c4-127">Para User: user. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="8a8c4-127">For user: User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="8a8c4-128">Para Device: Device. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="8a8c4-128">For device: Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="8a8c4-129">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a8c4-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a8c4-130">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-130">Not supported.</span></span> |
| <span data-ttu-id="8a8c4-131">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a8c4-131">Application</span></span>                            | <span data-ttu-id="8a8c4-132">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-132">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a8c4-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a8c4-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a><span data-ttu-id="8a8c4-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a8c4-134">Request headers</span></span>

| <span data-ttu-id="8a8c4-135">Nome</span><span class="sxs-lookup"><span data-stu-id="8a8c4-135">Name</span></span> | <span data-ttu-id="8a8c4-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a8c4-136">Description</span></span> |
| :--- | :---------- |
| <span data-ttu-id="8a8c4-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a8c4-137">Authorization</span></span> | <span data-ttu-id="8a8c4-138">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8a8c4-138">Bearer {token}</span></span> |
| <span data-ttu-id="8a8c4-139">Content-type</span><span class="sxs-lookup"><span data-stu-id="8a8c4-139">Content-type</span></span>  | <span data-ttu-id="8a8c4-140">application/json</span><span class="sxs-lookup"><span data-stu-id="8a8c4-140">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a8c4-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a8c4-141">Request body</span></span>

<span data-ttu-id="8a8c4-142">No corpo da solicitação, forneça as propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-142">In the request body, supply the required properties.</span></span>

<span data-ttu-id="8a8c4-143">A tabela a seguir lista as propriedades que são necessárias ao avaliar a associação de grupo.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-143">The following table lists the properties that are required when you evaluate group membership.</span></span>

| <span data-ttu-id="8a8c4-144">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8a8c4-144">Parameter</span></span> | <span data-ttu-id="8a8c4-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a8c4-145">Type</span></span> | <span data-ttu-id="8a8c4-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a8c4-146">Description</span></span> |
| :-------- | :--- | :---------- |
| <span data-ttu-id="8a8c4-147">MemberId</span><span class="sxs-lookup"><span data-stu-id="8a8c4-147">memberId</span></span> | <span data-ttu-id="8a8c4-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a8c4-148">String collection</span></span> | <span data-ttu-id="8a8c4-149">MemberId é a ID do objeto do usuário ou do dispositivo a ser avaliado.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-149">memberId is the object Id of the user or device to be evaluated.</span></span> |
| <span data-ttu-id="8a8c4-150">membershipRule</span><span class="sxs-lookup"><span data-stu-id="8a8c4-150">membershipRule</span></span> | <span data-ttu-id="8a8c4-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a8c4-151">String collection</span></span> | <span data-ttu-id="8a8c4-152">A regra usada para avaliação de associação.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-152">The rule that is used for membership evaluation.</span></span> <span data-ttu-id="8a8c4-153">Se essa propriedade não for fornecida, a regra do grupo existente será avaliada.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-153">If this property is not provided, the rule for the existing group is evaluated.</span></span> <span data-ttu-id="8a8c4-154">Se essa propriedade for fornecida, o usuário ou dispositivo será avaliado para uma possível associação em um grupo com a mesma regra.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-154">If this property is provided, the user or device is evaluated for possible membership in a group with the same rule.</span></span> <span data-ttu-id="8a8c4-155">Para obter mais informações, consulte [regras de associação dinâmicas para grupos no Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span><span class="sxs-lookup"><span data-stu-id="8a8c4-155">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span>|

## <a name="response"></a><span data-ttu-id="8a8c4-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a8c4-156">Response</span></span>

<span data-ttu-id="8a8c4-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) .</span><span class="sxs-lookup"><span data-stu-id="8a8c4-157">If successful, this method returns a `200 OK` response code and an [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="8a8c4-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8a8c4-158">Examples</span></span>

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a><span data-ttu-id="8a8c4-159">Exemplo 1: avaliar se um usuário ou dispositivo é um membro de um grupo existente</span><span class="sxs-lookup"><span data-stu-id="8a8c4-159">Example 1: Evaluate if a user or device is a member of an existing group</span></span>

#### <a name="request"></a><span data-ttu-id="8a8c4-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a8c4-160">Request</span></span>

<span data-ttu-id="8a8c4-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8a8c4-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a8c4-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33"
}
```
# <a name="c"></a>[<span data-ttu-id="8a8c4-163">C#</span><span class="sxs-lookup"><span data-stu-id="8a8c4-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a8c4-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a8c4-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a8c4-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a8c4-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a8c4-166">Java</span><span class="sxs-lookup"><span data-stu-id="8a8c4-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8a8c4-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a8c4-167">Response</span></span>

<span data-ttu-id="8a8c4-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-168">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}

```

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a><span data-ttu-id="8a8c4-169">Exemplo 2: avaliar se um usuário ou dispositivo é membro de um grupo com base em uma regra de associação</span><span class="sxs-lookup"><span data-stu-id="8a8c4-169">Example 2: Evaluate if a user or device would be a member of a group based on a membership rule</span></span>

#### <a name="request"></a><span data-ttu-id="8a8c4-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a8c4-170">Request</span></span>

<span data-ttu-id="8a8c4-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8a8c4-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a8c4-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership"
}-->

```http
POST https://graph.microsoft.com/beta/groups/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33",
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")"
}
```
# <a name="c"></a>[<span data-ttu-id="8a8c4-173">C#</span><span class="sxs-lookup"><span data-stu-id="8a8c4-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a8c4-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a8c4-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a8c4-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a8c4-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a8c4-176">Java</span><span class="sxs-lookup"><span data-stu-id="8a8c4-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8a8c4-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a8c4-177">Response</span></span>

<span data-ttu-id="8a8c4-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8a8c4-178">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: evaluateDynamicMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
