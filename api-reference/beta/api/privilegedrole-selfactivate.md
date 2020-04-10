---
title: 'privilegedRole: selfActivate'
description: Ative a função que é atribuída ao solicitante.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 79891be7aa63269cb0d1f96393756f9d41d046d0
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218749"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="ad152-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="ad152-103">privilegedRole: selfActivate</span></span>

<span data-ttu-id="ad152-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad152-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad152-105">Ative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="ad152-105">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="ad152-106">**Observação:** A partir de dezembro de 2018, esta API não terá mais suporte e não deve ser usada.</span><span class="sxs-lookup"><span data-stu-id="ad152-106">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="ad152-107">Use a [criar PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="ad152-107">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="ad152-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad152-108">Permissions</span></span>
<span data-ttu-id="ad152-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad152-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ad152-111">O solicitante só pode chamar ```selfActivate``` a função que é atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="ad152-111">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="ad152-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad152-112">Permission type</span></span>      | <span data-ttu-id="ad152-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad152-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad152-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad152-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ad152-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad152-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad152-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad152-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad152-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad152-117">Not supported.</span></span>    |
|<span data-ttu-id="ad152-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad152-118">Application</span></span> | <span data-ttu-id="ad152-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad152-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad152-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad152-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="ad152-121">Observe que ``{id}`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="ad152-121">Note that ``{id}`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ad152-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad152-122">Request headers</span></span>
| <span data-ttu-id="ad152-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ad152-123">Name</span></span>       | <span data-ttu-id="ad152-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad152-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ad152-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad152-125">Authorization</span></span>  | <span data-ttu-id="ad152-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad152-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad152-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad152-128">Request body</span></span>
<span data-ttu-id="ad152-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad152-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ad152-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ad152-130">Parameter</span></span>    | <span data-ttu-id="ad152-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad152-131">Type</span></span>   |<span data-ttu-id="ad152-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad152-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad152-133">motivo</span><span class="sxs-lookup"><span data-stu-id="ad152-133">reason</span></span>|<span data-ttu-id="ad152-134">string</span><span class="sxs-lookup"><span data-stu-id="ad152-134">string</span></span>|<span data-ttu-id="ad152-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ad152-135">Optional.</span></span> <span data-ttu-id="ad152-136">Descrição sobre o motivo para esta ativação de função.</span><span class="sxs-lookup"><span data-stu-id="ad152-136">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="ad152-137">duration</span><span class="sxs-lookup"><span data-stu-id="ad152-137">duration</span></span>|<span data-ttu-id="ad152-138">string</span><span class="sxs-lookup"><span data-stu-id="ad152-138">string</span></span>|<span data-ttu-id="ad152-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ad152-139">Optional.</span></span> <span data-ttu-id="ad152-140">Os valores válidos podem ```min``` ser (duração mínima da ativação ```default``` ), (duração de ativação padrão para a função) ou um valor duplo para especificar quantas horas é a ativação.</span><span class="sxs-lookup"><span data-stu-id="ad152-140">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="ad152-141">A duração especificada não pode ser maior do que a duração de ativação da função da configuração de função.</span><span class="sxs-lookup"><span data-stu-id="ad152-141">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="ad152-142">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="ad152-142">ticketNumber</span></span>|<span data-ttu-id="ad152-143">string</span><span class="sxs-lookup"><span data-stu-id="ad152-143">string</span></span>|<span data-ttu-id="ad152-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ad152-144">Optional.</span></span> <span data-ttu-id="ad152-145">O número do tíquete usado para controlar esta ativação de função.</span><span class="sxs-lookup"><span data-stu-id="ad152-145">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="ad152-146">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="ad152-146">ticketSystem</span></span>|<span data-ttu-id="ad152-147">string</span><span class="sxs-lookup"><span data-stu-id="ad152-147">string</span></span>|<span data-ttu-id="ad152-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ad152-148">Optional.</span></span> <span data-ttu-id="ad152-149">O sistema de permissão.</span><span class="sxs-lookup"><span data-stu-id="ad152-149">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="ad152-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad152-150">Response</span></span>

<span data-ttu-id="ad152-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad152-151">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="ad152-152">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="ad152-152">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ad152-153">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="ad152-153">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="ad152-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad152-154">Example</span></span>
<span data-ttu-id="ad152-155">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="ad152-155">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ad152-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad152-156">Request</span></span>
<span data-ttu-id="ad152-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad152-157">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad152-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad152-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ad152-159">C#</span><span class="sxs-lookup"><span data-stu-id="ad152-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad152-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad152-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad152-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad152-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ad152-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad152-162">Response</span></span>
<span data-ttu-id="ad152-163">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad152-163">Here is an example of the response.</span></span> 

><span data-ttu-id="ad152-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad152-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
