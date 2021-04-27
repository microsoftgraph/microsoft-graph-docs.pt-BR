---
title: 'privilegedRoleAssignment: makeEligible'
description: Tornar a atribuição de função qualificada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 97daaea03d58d73ab687380dd221d3e300b446c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037435"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="ca963-103">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="ca963-103">privilegedRoleAssignment: makeEligible</span></span>

<span data-ttu-id="ca963-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca963-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca963-105">Tornar a atribuição de função qualificada.</span><span class="sxs-lookup"><span data-stu-id="ca963-105">Make the role assignment eligible.</span></span> <span data-ttu-id="ca963-106">Se a atribuição de função já estiver qualificada antes da chamada, ela não faz nada.</span><span class="sxs-lookup"><span data-stu-id="ca963-106">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="ca963-107">Se a atribuição de função for permanente e o solicitante for diferente do usuário de destino, a atribuição de função se tornará qualificada e a função será desativada para o usuário de destino.</span><span class="sxs-lookup"><span data-stu-id="ca963-107">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="ca963-108">Se o solicitante for o usuário de destino e a função for Administrador de Segurança ou Administrador de Função Privilegiada, a função será ativada com a expiração padrão.</span><span class="sxs-lookup"><span data-stu-id="ca963-108">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca963-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca963-109">Permissions</span></span>
<span data-ttu-id="ca963-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca963-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ca963-112">O solicitante precisa ter função _de Administrador de Função_ Privilegiada.</span><span class="sxs-lookup"><span data-stu-id="ca963-112">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="ca963-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca963-113">Permission type</span></span>      | <span data-ttu-id="ca963-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca963-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca963-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca963-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ca963-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca963-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca963-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca963-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca963-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca963-118">Not supported.</span></span>    |
|<span data-ttu-id="ca963-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca963-119">Application</span></span> | <span data-ttu-id="ca963-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca963-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca963-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca963-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="ca963-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca963-122">Request headers</span></span>
| <span data-ttu-id="ca963-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ca963-123">Name</span></span>       | <span data-ttu-id="ca963-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca963-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ca963-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca963-125">Authorization</span></span>  | <span data-ttu-id="ca963-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca963-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca963-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca963-128">Request body</span></span>
<span data-ttu-id="ca963-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca963-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca963-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca963-130">Response</span></span>

<span data-ttu-id="ca963-131">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca963-131">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="ca963-132">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="ca963-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ca963-133">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="ca963-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="ca963-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca963-134">Example</span></span>
<span data-ttu-id="ca963-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ca963-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ca963-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca963-136">Request</span></span>
<span data-ttu-id="ca963-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca963-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca963-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca963-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```
# <a name="c"></a>[<span data-ttu-id="ca963-139">C#</span><span class="sxs-lookup"><span data-stu-id="ca963-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makeeligible-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca963-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca963-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makeeligible-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca963-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca963-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makeeligible-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca963-142">Java</span><span class="sxs-lookup"><span data-stu-id="ca963-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makeeligible-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ca963-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca963-143">Response</span></span>
<span data-ttu-id="ca963-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca963-144">Here is an example of the response.</span></span> <span data-ttu-id="ca963-145">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ca963-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


