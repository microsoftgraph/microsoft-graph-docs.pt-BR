---
title: 'group: evaluateDynamicMembership'
description: Avalie se um usuário ou dispositivo é ou seria membro de um grupo dinâmico.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: de8e44a79644bcea5e3c44b214580e16359468e2
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681757"
---
# <a name="group-evaluatedynamicmembership"></a><span data-ttu-id="eb831-103">group: evaluateDynamicMembership</span><span class="sxs-lookup"><span data-stu-id="eb831-103">group: evaluateDynamicMembership</span></span>

<span data-ttu-id="eb831-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb831-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb831-105">Avaliar se um usuário ou dispositivo é ou seria membro de um grupo dinâmico.</span><span class="sxs-lookup"><span data-stu-id="eb831-105">Evaluate whether a user or device is or would be a member of a dynamic group.</span></span> <span data-ttu-id="eb831-106">A regra de associação é retornada juntamente com outros detalhes que foram usados na avaliação.</span><span class="sxs-lookup"><span data-stu-id="eb831-106">The membership rule is returned along with other details that were used in the evaluation.</span></span> <span data-ttu-id="eb831-107">Você pode concluir essa operação das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="eb831-107">You can complete this operation in the following ways:</span></span> 

- <span data-ttu-id="eb831-108">Avalie se um usuário ou dispositivo é membro de um grupo dinâmico especificado.</span><span class="sxs-lookup"><span data-stu-id="eb831-108">Evaluate whether a user or device is a member of a specified dynamic group.</span></span>  
- <span data-ttu-id="eb831-109">Avalie se um usuário ou dispositivo seria membro de um grupo dinâmico com base na ID do usuário ou dispositivo e uma regra de associação.</span><span class="sxs-lookup"><span data-stu-id="eb831-109">Evaluate whether a user or device would be a member of a dynamic group based on the ID of the user or device and a membership rule.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb831-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb831-110">Permissions</span></span>

<span data-ttu-id="eb831-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb831-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a><span data-ttu-id="eb831-113">Avaliar a associação dinâmica com a ID do membro e a ID do grupo</span><span class="sxs-lookup"><span data-stu-id="eb831-113">Evaluate dynamic membership with member ID and group ID</span></span>

| <span data-ttu-id="eb831-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb831-114">Permission type</span></span> | <span data-ttu-id="eb831-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb831-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="eb831-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb831-116">Delegated (work or school account)</span></span> | <span data-ttu-id="eb831-117">Para usuário: Group.Read.All e User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb831-117">For user: Group.Read.All and User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="eb831-118">Para dispositivo: Group.Read.All e Device.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb831-118">For device: Group.Read.All and Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="eb831-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb831-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb831-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb831-120">Not supported.</span></span> |
| <span data-ttu-id="eb831-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb831-121">Application</span></span>                            | <span data-ttu-id="eb831-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb831-122">Not supported.</span></span> |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a><span data-ttu-id="eb831-123">Avaliar a associação dinâmica com a ID do membro e a regra de associação</span><span class="sxs-lookup"><span data-stu-id="eb831-123">Evaluate dynamic membership with member ID and membership rule</span></span>

| <span data-ttu-id="eb831-124">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb831-124">Permission type</span></span> | <span data-ttu-id="eb831-125">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb831-125">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="eb831-126">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb831-126">Delegated (work or school account)</span></span> | <span data-ttu-id="eb831-127">Para usuário: User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb831-127">For user: User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="eb831-128">Para dispositivo: Device.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb831-128">For device: Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="eb831-129">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb831-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb831-130">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb831-130">Not supported.</span></span> |
| <span data-ttu-id="eb831-131">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb831-131">Application</span></span>                            | <span data-ttu-id="eb831-132">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb831-132">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb831-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb831-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a><span data-ttu-id="eb831-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb831-134">Request headers</span></span>

| <span data-ttu-id="eb831-135">Nome</span><span class="sxs-lookup"><span data-stu-id="eb831-135">Name</span></span> | <span data-ttu-id="eb831-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb831-136">Description</span></span> |
| :--- | :---------- |
| <span data-ttu-id="eb831-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb831-137">Authorization</span></span> | <span data-ttu-id="eb831-138">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="eb831-138">Bearer {token}</span></span> |
| <span data-ttu-id="eb831-139">Content-type</span><span class="sxs-lookup"><span data-stu-id="eb831-139">Content-type</span></span>  | <span data-ttu-id="eb831-140">application/json</span><span class="sxs-lookup"><span data-stu-id="eb831-140">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb831-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb831-141">Request body</span></span>

<span data-ttu-id="eb831-142">No corpo da solicitação, fornece as propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="eb831-142">In the request body, supply the required properties.</span></span>

<span data-ttu-id="eb831-143">A tabela a seguir lista as propriedades necessárias ao avaliar a associação ao grupo.</span><span class="sxs-lookup"><span data-stu-id="eb831-143">The following table lists the properties that are required when you evaluate group membership.</span></span>

| <span data-ttu-id="eb831-144">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="eb831-144">Parameter</span></span> | <span data-ttu-id="eb831-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb831-145">Type</span></span> | <span data-ttu-id="eb831-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb831-146">Description</span></span> |
| :-------- | :--- | :---------- |
| <span data-ttu-id="eb831-147">memberId</span><span class="sxs-lookup"><span data-stu-id="eb831-147">memberId</span></span> | <span data-ttu-id="eb831-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb831-148">String collection</span></span> | <span data-ttu-id="eb831-149">memberId é a ID do objeto do usuário ou dispositivo a ser avaliado.</span><span class="sxs-lookup"><span data-stu-id="eb831-149">memberId is the object Id of the user or device to be evaluated.</span></span> |
| <span data-ttu-id="eb831-150">membershipRule</span><span class="sxs-lookup"><span data-stu-id="eb831-150">membershipRule</span></span> | <span data-ttu-id="eb831-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb831-151">String collection</span></span> | <span data-ttu-id="eb831-152">A regra usada para avaliação de associação.</span><span class="sxs-lookup"><span data-stu-id="eb831-152">The rule that is used for membership evaluation.</span></span> <span data-ttu-id="eb831-153">Se essa propriedade não for fornecida, a regra do grupo existente será avaliada.</span><span class="sxs-lookup"><span data-stu-id="eb831-153">If this property is not provided, the rule for the existing group is evaluated.</span></span> <span data-ttu-id="eb831-154">Se essa propriedade for fornecida, o usuário ou dispositivo será avaliado para possível associação em um grupo com a mesma regra.</span><span class="sxs-lookup"><span data-stu-id="eb831-154">If this property is provided, the user or device is evaluated for possible membership in a group with the same rule.</span></span> <span data-ttu-id="eb831-155">Para obter mais informações, consulte [Regras de associação dinâmicas para grupos em Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span><span class="sxs-lookup"><span data-stu-id="eb831-155">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span>|

## <a name="response"></a><span data-ttu-id="eb831-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb831-156">Response</span></span>

<span data-ttu-id="eb831-157">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [evaluateDynamicMembershipResult.](../resources/evaluatedynamicmembershipresult.md)</span><span class="sxs-lookup"><span data-stu-id="eb831-157">If successful, this method returns a `200 OK` response code and an [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="eb831-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eb831-158">Examples</span></span>

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a><span data-ttu-id="eb831-159">Exemplo 1: Avaliar se um usuário ou dispositivo é membro de um grupo existente</span><span class="sxs-lookup"><span data-stu-id="eb831-159">Example 1: Evaluate if a user or device is a member of an existing group</span></span>

#### <a name="request"></a><span data-ttu-id="eb831-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb831-160">Request</span></span>

<span data-ttu-id="eb831-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb831-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb831-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb831-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_1"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33"
}
```
# <a name="c"></a>[<span data-ttu-id="eb831-163">C#</span><span class="sxs-lookup"><span data-stu-id="eb831-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb831-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb831-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb831-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb831-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb831-166">Java</span><span class="sxs-lookup"><span data-stu-id="eb831-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eb831-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb831-167">Response</span></span>

<span data-ttu-id="eb831-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb831-168">The following is an example of the response.</span></span> 

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

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a><span data-ttu-id="eb831-169">Exemplo 2: Avaliar se um usuário ou dispositivo seria um membro de um grupo com base em uma regra de associação</span><span class="sxs-lookup"><span data-stu-id="eb831-169">Example 2: Evaluate if a user or device would be a member of a group based on a membership rule</span></span>

#### <a name="request"></a><span data-ttu-id="eb831-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb831-170">Request</span></span>

<span data-ttu-id="eb831-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb831-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb831-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb831-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_2"
}-->

```http
POST https://graph.microsoft.com/beta/groups/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33",
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")"
}
```
# <a name="c"></a>[<span data-ttu-id="eb831-173">C#</span><span class="sxs-lookup"><span data-stu-id="eb831-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb831-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb831-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb831-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb831-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb831-176">Java</span><span class="sxs-lookup"><span data-stu-id="eb831-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eb831-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb831-177">Response</span></span>

<span data-ttu-id="eb831-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb831-178">The following is an example of the response.</span></span> 

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
