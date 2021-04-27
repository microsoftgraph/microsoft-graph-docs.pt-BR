---
title: 'privilegedRole: selfActivate'
description: Ative a função atribuída ao solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 970435589de932ad10051196ef51da8764444260
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055250"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="cb528-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="cb528-103">privilegedRole: selfActivate</span></span>

<span data-ttu-id="cb528-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb528-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb528-105">Ative a função atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="cb528-105">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="cb528-106">**Observação:** A partir de dezembro de 2018, essa API não terá mais suporte e não deverá ser usada.</span><span class="sxs-lookup"><span data-stu-id="cb528-106">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="cb528-107">Em vez [disso, use Create PrivilegedRoleAssignmentRequest.](privilegedroleassignmentrequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="cb528-107">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="cb528-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb528-108">Permissions</span></span>
<span data-ttu-id="cb528-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb528-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cb528-111">O solicitante só pode ```selfActivate``` chamar a função atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="cb528-111">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="cb528-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb528-112">Permission type</span></span>      | <span data-ttu-id="cb528-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb528-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb528-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb528-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cb528-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb528-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cb528-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb528-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb528-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb528-117">Not supported.</span></span>    |
|<span data-ttu-id="cb528-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb528-118">Application</span></span> | <span data-ttu-id="cb528-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb528-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb528-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb528-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="cb528-121">Observe que ``{id}`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="cb528-121">Note that ``{id}`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cb528-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb528-122">Request headers</span></span>
| <span data-ttu-id="cb528-123">Nome</span><span class="sxs-lookup"><span data-stu-id="cb528-123">Name</span></span>       | <span data-ttu-id="cb528-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb528-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cb528-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb528-125">Authorization</span></span>  | <span data-ttu-id="cb528-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb528-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb528-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb528-128">Request body</span></span>
<span data-ttu-id="cb528-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb528-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cb528-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cb528-130">Parameter</span></span>    | <span data-ttu-id="cb528-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb528-131">Type</span></span>   |<span data-ttu-id="cb528-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb528-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb528-133">motivo</span><span class="sxs-lookup"><span data-stu-id="cb528-133">reason</span></span>|<span data-ttu-id="cb528-134">string</span><span class="sxs-lookup"><span data-stu-id="cb528-134">string</span></span>|<span data-ttu-id="cb528-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cb528-135">Optional.</span></span> <span data-ttu-id="cb528-136">Descrição sobre o motivo da ativação dessa função.</span><span class="sxs-lookup"><span data-stu-id="cb528-136">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="cb528-137">duração</span><span class="sxs-lookup"><span data-stu-id="cb528-137">duration</span></span>|<span data-ttu-id="cb528-138">string</span><span class="sxs-lookup"><span data-stu-id="cb528-138">string</span></span>|<span data-ttu-id="cb528-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cb528-139">Optional.</span></span> <span data-ttu-id="cb528-140">Os valores válidos podem ser (duração mínima de ativação), (duração de ativação padrão para a função) ou um valor duplo para especificar quantas horas ```min``` ```default``` é a ativação.</span><span class="sxs-lookup"><span data-stu-id="cb528-140">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="cb528-141">A duração especificada não pode ser maior do que a duração de ativação da função na configuração da função.</span><span class="sxs-lookup"><span data-stu-id="cb528-141">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="cb528-142">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="cb528-142">ticketNumber</span></span>|<span data-ttu-id="cb528-143">string</span><span class="sxs-lookup"><span data-stu-id="cb528-143">string</span></span>|<span data-ttu-id="cb528-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cb528-144">Optional.</span></span> <span data-ttu-id="cb528-145">O número do tíquete usado para controlar essa ativação de função.</span><span class="sxs-lookup"><span data-stu-id="cb528-145">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="cb528-146">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="cb528-146">ticketSystem</span></span>|<span data-ttu-id="cb528-147">string</span><span class="sxs-lookup"><span data-stu-id="cb528-147">string</span></span>|<span data-ttu-id="cb528-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cb528-148">Optional.</span></span> <span data-ttu-id="cb528-149">O sistema de tíquetes.</span><span class="sxs-lookup"><span data-stu-id="cb528-149">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="cb528-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb528-150">Response</span></span>

<span data-ttu-id="cb528-151">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb528-151">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="cb528-152">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="cb528-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="cb528-153">Caso contrário, o código de status HTTP 403 Forbidden será retornado.</span><span class="sxs-lookup"><span data-stu-id="cb528-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="cb528-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb528-154">Example</span></span>
<span data-ttu-id="cb528-155">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="cb528-155">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cb528-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb528-156">Request</span></span>
<span data-ttu-id="cb528-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb528-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cb528-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb528-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cb528-159">C#</span><span class="sxs-lookup"><span data-stu-id="cb528-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb528-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb528-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb528-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb528-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb528-162">Java</span><span class="sxs-lookup"><span data-stu-id="cb528-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedrole-selfactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cb528-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb528-163">Response</span></span>
<span data-ttu-id="cb528-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb528-164">Here is an example of the response.</span></span> 

><span data-ttu-id="cb528-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cb528-165">**Note:** The response object shown here might be shortened for readability.</span></span>
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


