---
title: 'privilegedRoleAssignment: makePermanent'
description: Torne a atribuição de função como permanente.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b17cb3d7bb1248be06d34078f0f0bc897870c684
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455330"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="d5e2f-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="d5e2f-103">privilegedRoleAssignment: makePermanent</span></span>

<span data-ttu-id="d5e2f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d5e2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5e2f-105">Torne a atribuição de função como permanente.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-105">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5e2f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5e2f-106">Permissions</span></span>
<span data-ttu-id="d5e2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5e2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d5e2f-109">O locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-109">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d5e2f-110">Caso contrário, o erro HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-110">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="d5e2f-111">O solicitante precisa ter função de _administrador de função privilegiada_ .</span><span class="sxs-lookup"><span data-stu-id="d5e2f-111">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="d5e2f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5e2f-112">Permission type</span></span>      | <span data-ttu-id="d5e2f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5e2f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5e2f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5e2f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d5e2f-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d5e2f-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d5e2f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5e2f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5e2f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-117">Not supported.</span></span>    |
|<span data-ttu-id="d5e2f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5e2f-118">Application</span></span> | <span data-ttu-id="d5e2f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5e2f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e2f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="d5e2f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5e2f-121">Request headers</span></span>
| <span data-ttu-id="d5e2f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d5e2f-122">Name</span></span>       | <span data-ttu-id="d5e2f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5e2f-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d5e2f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5e2f-124">Authorization</span></span>  | <span data-ttu-id="d5e2f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5e2f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5e2f-127">Request body</span></span>
<span data-ttu-id="d5e2f-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d5e2f-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5e2f-129">Parameter</span></span>    | <span data-ttu-id="d5e2f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5e2f-130">Type</span></span>   |<span data-ttu-id="d5e2f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5e2f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5e2f-132">motivo</span><span class="sxs-lookup"><span data-stu-id="d5e2f-132">reason</span></span>|<span data-ttu-id="d5e2f-133">string</span><span class="sxs-lookup"><span data-stu-id="d5e2f-133">string</span></span>|<span data-ttu-id="d5e2f-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-134">Optional.</span></span> <span data-ttu-id="d5e2f-135">O motivo para fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-135">The reason to make this call.</span></span>|
|<span data-ttu-id="d5e2f-136">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="d5e2f-136">ticketNumber</span></span>|<span data-ttu-id="d5e2f-137">string</span><span class="sxs-lookup"><span data-stu-id="d5e2f-137">string</span></span>|<span data-ttu-id="d5e2f-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-138">Optional.</span></span> <span data-ttu-id="d5e2f-139">O número do tíquete associado a esta ação.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-139">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="d5e2f-140">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="d5e2f-140">ticketSystem</span></span>|<span data-ttu-id="d5e2f-141">string</span><span class="sxs-lookup"><span data-stu-id="d5e2f-141">string</span></span>|<span data-ttu-id="d5e2f-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-142">Optional.</span></span> <span data-ttu-id="d5e2f-143">O sistema de permissão.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-143">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="d5e2f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5e2f-144">Response</span></span>

<span data-ttu-id="d5e2f-145">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-145">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5e2f-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5e2f-146">Example</span></span>
<span data-ttu-id="d5e2f-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d5e2f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5e2f-148">Request</span></span>
<span data-ttu-id="d5e2f-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5e2f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e2f-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d5e2f-151">C#</span><span class="sxs-lookup"><span data-stu-id="d5e2f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makepermanent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5e2f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5e2f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makepermanent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5e2f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5e2f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makepermanent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d5e2f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5e2f-154">Response</span></span>
<span data-ttu-id="d5e2f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5e2f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
