---
title: 'privilegedRoleAssignment: makePermanent'
description: Tornar a atribuição de função permanente.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: c457cc3c70e1a3f7cafec9a929c68ed3b7fddcea
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441197"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="eb2b2-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="eb2b2-103">privilegedRoleAssignment: makePermanent</span></span>

<span data-ttu-id="eb2b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb2b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb2b2-105">Tornar a atribuição de função permanente.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-105">Make the role assignment permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb2b2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb2b2-106">Permissions</span></span>
<span data-ttu-id="eb2b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb2b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="eb2b2-109">O locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-109">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="eb2b2-110">Caso contrário, o erro HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-110">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="eb2b2-111">O solicitante precisa ter função _de Administrador de Função_ Privilegiada.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-111">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="eb2b2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb2b2-112">Permission type</span></span>      | <span data-ttu-id="eb2b2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb2b2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb2b2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb2b2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="eb2b2-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eb2b2-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eb2b2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb2b2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb2b2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-117">Not supported.</span></span>    |
|<span data-ttu-id="eb2b2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb2b2-118">Application</span></span> | <span data-ttu-id="eb2b2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb2b2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb2b2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="eb2b2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb2b2-121">Request headers</span></span>
| <span data-ttu-id="eb2b2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="eb2b2-122">Name</span></span>       | <span data-ttu-id="eb2b2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb2b2-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eb2b2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb2b2-124">Authorization</span></span>  | <span data-ttu-id="eb2b2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb2b2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb2b2-127">Request body</span></span>
<span data-ttu-id="eb2b2-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eb2b2-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="eb2b2-129">Parameter</span></span>    | <span data-ttu-id="eb2b2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb2b2-130">Type</span></span>   |<span data-ttu-id="eb2b2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb2b2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb2b2-132">motivo</span><span class="sxs-lookup"><span data-stu-id="eb2b2-132">reason</span></span>|<span data-ttu-id="eb2b2-133">string</span><span class="sxs-lookup"><span data-stu-id="eb2b2-133">string</span></span>|<span data-ttu-id="eb2b2-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-134">Optional.</span></span> <span data-ttu-id="eb2b2-135">O motivo para fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-135">The reason to make this call.</span></span>|
|<span data-ttu-id="eb2b2-136">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="eb2b2-136">ticketNumber</span></span>|<span data-ttu-id="eb2b2-137">string</span><span class="sxs-lookup"><span data-stu-id="eb2b2-137">string</span></span>|<span data-ttu-id="eb2b2-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-138">Optional.</span></span> <span data-ttu-id="eb2b2-139">O número do tíquete associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-139">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="eb2b2-140">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="eb2b2-140">ticketSystem</span></span>|<span data-ttu-id="eb2b2-141">string</span><span class="sxs-lookup"><span data-stu-id="eb2b2-141">string</span></span>|<span data-ttu-id="eb2b2-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-142">Optional.</span></span> <span data-ttu-id="eb2b2-143">O sistema de tíquetes.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-143">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="eb2b2-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb2b2-144">Response</span></span>

<span data-ttu-id="eb2b2-145">Se tiver êxito, este método retornará `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-145">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb2b2-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb2b2-146">Example</span></span>
<span data-ttu-id="eb2b2-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eb2b2-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb2b2-148">Request</span></span>
<span data-ttu-id="eb2b2-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eb2b2-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb2b2-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eb2b2-151">C#</span><span class="sxs-lookup"><span data-stu-id="eb2b2-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makepermanent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb2b2-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb2b2-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makepermanent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb2b2-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb2b2-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makepermanent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb2b2-154">Java</span><span class="sxs-lookup"><span data-stu-id="eb2b2-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makepermanent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eb2b2-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb2b2-155">Response</span></span>
<span data-ttu-id="eb2b2-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb2b2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


