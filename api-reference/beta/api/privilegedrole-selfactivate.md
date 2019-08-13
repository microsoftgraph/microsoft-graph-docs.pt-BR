---
title: 'privilegedRole: selfActivate'
description: Ative a função que é atribuída ao solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7fbe9b8a0f37238c393d5c9848b578263b5318ae
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361228"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="f7684-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="f7684-103">privilegedRole: selfActivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7684-104">Ative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="f7684-104">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="f7684-105">**Observação:** A partir de dezembro de 2018, esta API não terá mais suporte e não deve ser usada.</span><span class="sxs-lookup"><span data-stu-id="f7684-105">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="f7684-106">Use a [criar PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="f7684-106">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="f7684-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7684-107">Permissions</span></span>
<span data-ttu-id="f7684-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7684-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f7684-110">O solicitante só pode chamar ```selfActivate``` a função que é atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="f7684-110">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="f7684-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7684-111">Permission type</span></span>      | <span data-ttu-id="f7684-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7684-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7684-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7684-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f7684-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f7684-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f7684-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7684-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7684-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7684-116">Not supported.</span></span>    |
|<span data-ttu-id="f7684-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7684-117">Application</span></span> | <span data-ttu-id="f7684-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7684-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7684-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7684-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="f7684-120">Observe que ``<id>`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="f7684-120">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f7684-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7684-121">Request headers</span></span>
| <span data-ttu-id="f7684-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f7684-122">Name</span></span>       | <span data-ttu-id="f7684-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7684-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7684-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7684-124">Authorization</span></span>  | <span data-ttu-id="f7684-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7684-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7684-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7684-127">Request body</span></span>
<span data-ttu-id="f7684-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7684-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7684-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f7684-129">Parameter</span></span>    | <span data-ttu-id="f7684-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7684-130">Type</span></span>   |<span data-ttu-id="f7684-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7684-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7684-132">motivos</span><span class="sxs-lookup"><span data-stu-id="f7684-132">reason</span></span>|<span data-ttu-id="f7684-133">string</span><span class="sxs-lookup"><span data-stu-id="f7684-133">string</span></span>|<span data-ttu-id="f7684-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f7684-134">Optional.</span></span> <span data-ttu-id="f7684-135">Descrição sobre o motivo para esta ativação de função.</span><span class="sxs-lookup"><span data-stu-id="f7684-135">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="f7684-136">duration</span><span class="sxs-lookup"><span data-stu-id="f7684-136">duration</span></span>|<span data-ttu-id="f7684-137">string</span><span class="sxs-lookup"><span data-stu-id="f7684-137">string</span></span>|<span data-ttu-id="f7684-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f7684-138">Optional.</span></span> <span data-ttu-id="f7684-139">Os valores válidos podem ```min``` ser (duração mínima da ativação ```default``` ), (duração de ativação padrão para a função) ou um valor duplo para especificar quantas horas é a ativação.</span><span class="sxs-lookup"><span data-stu-id="f7684-139">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="f7684-140">A duração especificada não pode ser maior do que a duração de ativação da função da configuração de função.</span><span class="sxs-lookup"><span data-stu-id="f7684-140">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="f7684-141">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="f7684-141">ticketNumber</span></span>|<span data-ttu-id="f7684-142">string</span><span class="sxs-lookup"><span data-stu-id="f7684-142">string</span></span>|<span data-ttu-id="f7684-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f7684-143">Optional.</span></span> <span data-ttu-id="f7684-144">O número do tíquete usado para controlar esta ativação de função.</span><span class="sxs-lookup"><span data-stu-id="f7684-144">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="f7684-145">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="f7684-145">ticketSystem</span></span>|<span data-ttu-id="f7684-146">string</span><span class="sxs-lookup"><span data-stu-id="f7684-146">string</span></span>|<span data-ttu-id="f7684-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f7684-147">Optional.</span></span> <span data-ttu-id="f7684-148">O sistema de permissão.</span><span class="sxs-lookup"><span data-stu-id="f7684-148">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="f7684-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7684-149">Response</span></span>

<span data-ttu-id="f7684-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7684-150">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="f7684-151">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="f7684-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f7684-152">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="f7684-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="f7684-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7684-153">Example</span></span>
<span data-ttu-id="f7684-154">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f7684-154">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f7684-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7684-155">Request</span></span>
<span data-ttu-id="f7684-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7684-156">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f7684-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7684-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfActivate
Content-type: application/json
Content-length: 142

{
  "reason": "reason-value",
  "duration": "duration-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7684-158">C#</span><span class="sxs-lookup"><span data-stu-id="f7684-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7684-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7684-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7684-160">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f7684-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f7684-161">Java</span><span class="sxs-lookup"><span data-stu-id="f7684-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedrole-selfactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f7684-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7684-162">Response</span></span>
<span data-ttu-id="f7684-163">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7684-163">Here is an example of the response.</span></span> 

><span data-ttu-id="f7684-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7684-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
