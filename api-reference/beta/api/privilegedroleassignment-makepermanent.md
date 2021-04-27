---
title: 'privilegedRoleAssignment: makePermanent'
description: Tornar a atribuição de função permanente.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a66834f5937b8dea55391553536670ff06ae83c6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037372"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="58819-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="58819-103">privilegedRoleAssignment: makePermanent</span></span>

<span data-ttu-id="58819-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58819-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58819-105">Tornar a atribuição de função permanente.</span><span class="sxs-lookup"><span data-stu-id="58819-105">Make the role assignment permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="58819-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="58819-106">Permissions</span></span>
<span data-ttu-id="58819-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58819-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="58819-109">O locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="58819-109">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="58819-110">Caso contrário, o erro HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="58819-110">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="58819-111">O solicitante precisa ter função _de Administrador de Função_ Privilegiada.</span><span class="sxs-lookup"><span data-stu-id="58819-111">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="58819-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58819-112">Permission type</span></span>      | <span data-ttu-id="58819-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58819-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58819-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58819-114">Delegated (work or school account)</span></span> | <span data-ttu-id="58819-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="58819-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="58819-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58819-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58819-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58819-117">Not supported.</span></span>    |
|<span data-ttu-id="58819-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58819-118">Application</span></span> | <span data-ttu-id="58819-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58819-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58819-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58819-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="58819-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58819-121">Request headers</span></span>
| <span data-ttu-id="58819-122">Nome</span><span class="sxs-lookup"><span data-stu-id="58819-122">Name</span></span>       | <span data-ttu-id="58819-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="58819-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="58819-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="58819-124">Authorization</span></span>  | <span data-ttu-id="58819-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58819-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58819-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58819-127">Request body</span></span>
<span data-ttu-id="58819-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58819-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58819-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="58819-129">Parameter</span></span>    | <span data-ttu-id="58819-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="58819-130">Type</span></span>   |<span data-ttu-id="58819-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="58819-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58819-132">motivo</span><span class="sxs-lookup"><span data-stu-id="58819-132">reason</span></span>|<span data-ttu-id="58819-133">string</span><span class="sxs-lookup"><span data-stu-id="58819-133">string</span></span>|<span data-ttu-id="58819-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="58819-134">Optional.</span></span> <span data-ttu-id="58819-135">O motivo para fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="58819-135">The reason to make this call.</span></span>|
|<span data-ttu-id="58819-136">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="58819-136">ticketNumber</span></span>|<span data-ttu-id="58819-137">string</span><span class="sxs-lookup"><span data-stu-id="58819-137">string</span></span>|<span data-ttu-id="58819-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="58819-138">Optional.</span></span> <span data-ttu-id="58819-139">O número do tíquete associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="58819-139">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="58819-140">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="58819-140">ticketSystem</span></span>|<span data-ttu-id="58819-141">string</span><span class="sxs-lookup"><span data-stu-id="58819-141">string</span></span>|<span data-ttu-id="58819-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="58819-142">Optional.</span></span> <span data-ttu-id="58819-143">O sistema de tíquetes.</span><span class="sxs-lookup"><span data-stu-id="58819-143">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="58819-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="58819-144">Response</span></span>

<span data-ttu-id="58819-145">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58819-145">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58819-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58819-146">Example</span></span>
<span data-ttu-id="58819-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="58819-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="58819-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58819-148">Request</span></span>
<span data-ttu-id="58819-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58819-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58819-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="58819-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makepermanent"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makePermanent
Content-type: application/json
Content-length: 110

{
  "reason": "reason-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```
# <a name="c"></a>[<span data-ttu-id="58819-151">C#</span><span class="sxs-lookup"><span data-stu-id="58819-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makepermanent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58819-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58819-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makepermanent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58819-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58819-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makepermanent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58819-154">Java</span><span class="sxs-lookup"><span data-stu-id="58819-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makepermanent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="58819-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="58819-155">Response</span></span>
<span data-ttu-id="58819-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58819-156">Here is an example of the response.</span></span> <span data-ttu-id="58819-157">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="58819-157">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "privilegedRoleAssignment: makePermanent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


