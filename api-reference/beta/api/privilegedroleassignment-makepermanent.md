---
title: 'privilegedRoleAssignment: makePermanent'
description: Torne a atribuição de função como permanente.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7b1db98c98c1da5268b4019c20a3a1fe04851c74
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361059"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="ceeec-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="ceeec-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceeec-104">Torne a atribuição de função como permanente.</span><span class="sxs-lookup"><span data-stu-id="ceeec-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="ceeec-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ceeec-105">Permissions</span></span>
<span data-ttu-id="ceeec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceeec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ceeec-108">O locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="ceeec-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ceeec-109">Caso contrário, o erro HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="ceeec-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="ceeec-110">O solicitante precisa ter função de _administrador de função privilegiada_ .</span><span class="sxs-lookup"><span data-stu-id="ceeec-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="ceeec-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ceeec-111">Permission type</span></span>      | <span data-ttu-id="ceeec-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ceeec-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ceeec-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ceeec-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ceeec-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ceeec-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ceeec-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ceeec-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceeec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceeec-116">Not supported.</span></span>    |
|<span data-ttu-id="ceeec-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ceeec-117">Application</span></span> | <span data-ttu-id="ceeec-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceeec-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ceeec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceeec-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="ceeec-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceeec-120">Request headers</span></span>
| <span data-ttu-id="ceeec-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ceeec-121">Name</span></span>       | <span data-ttu-id="ceeec-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceeec-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ceeec-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceeec-123">Authorization</span></span>  | <span data-ttu-id="ceeec-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceeec-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ceeec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceeec-126">Request body</span></span>
<span data-ttu-id="ceeec-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceeec-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ceeec-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ceeec-128">Parameter</span></span>    | <span data-ttu-id="ceeec-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ceeec-129">Type</span></span>   |<span data-ttu-id="ceeec-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceeec-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ceeec-131">motivos</span><span class="sxs-lookup"><span data-stu-id="ceeec-131">reason</span></span>|<span data-ttu-id="ceeec-132">string</span><span class="sxs-lookup"><span data-stu-id="ceeec-132">string</span></span>|<span data-ttu-id="ceeec-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ceeec-133">Optional.</span></span> <span data-ttu-id="ceeec-134">O motivo para fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="ceeec-134">The reason to make this call.</span></span>|
|<span data-ttu-id="ceeec-135">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="ceeec-135">ticketNumber</span></span>|<span data-ttu-id="ceeec-136">string</span><span class="sxs-lookup"><span data-stu-id="ceeec-136">string</span></span>|<span data-ttu-id="ceeec-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ceeec-137">Optional.</span></span> <span data-ttu-id="ceeec-138">O número do tíquete associado a esta ação.</span><span class="sxs-lookup"><span data-stu-id="ceeec-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="ceeec-139">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="ceeec-139">ticketSystem</span></span>|<span data-ttu-id="ceeec-140">string</span><span class="sxs-lookup"><span data-stu-id="ceeec-140">string</span></span>|<span data-ttu-id="ceeec-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ceeec-141">Optional.</span></span> <span data-ttu-id="ceeec-142">O sistema de permissão.</span><span class="sxs-lookup"><span data-stu-id="ceeec-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="ceeec-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceeec-143">Response</span></span>

<span data-ttu-id="ceeec-144">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceeec-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceeec-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ceeec-145">Example</span></span>
<span data-ttu-id="ceeec-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ceeec-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ceeec-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceeec-147">Request</span></span>
<span data-ttu-id="ceeec-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceeec-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ceeec-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ceeec-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ceeec-150">C#</span><span class="sxs-lookup"><span data-stu-id="ceeec-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makepermanent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ceeec-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ceeec-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makepermanent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ceeec-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ceeec-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makepermanent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ceeec-153">Java</span><span class="sxs-lookup"><span data-stu-id="ceeec-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makepermanent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ceeec-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceeec-154">Response</span></span>
<span data-ttu-id="ceeec-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ceeec-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
