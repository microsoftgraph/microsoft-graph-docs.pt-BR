---
title: 'privilegedRole: selfActivate'
description: Ative a função que é atribuída ao solicitante.
localization_priority: Normal
ms.openlocfilehash: a6afd9d82536e5cd4660529ad44c064a487fa640
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594731"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="533e3-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="533e3-103">privilegedRole: selfActivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="533e3-104">Ative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="533e3-104">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="533e3-105">**Observação:** A partir de dezembro de 2018, esta API não terá mais suporte e não deve ser usada.</span><span class="sxs-lookup"><span data-stu-id="533e3-105">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="533e3-106">Use a [criar PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) em vez disso.</span><span class="sxs-lookup"><span data-stu-id="533e3-106">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="533e3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="533e3-107">Permissions</span></span>
<span data-ttu-id="533e3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="533e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="533e3-110">O solicitante só pode chamar ```selfActivate``` a função que é atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="533e3-110">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="533e3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="533e3-111">Permission type</span></span>      | <span data-ttu-id="533e3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="533e3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="533e3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="533e3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="533e3-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="533e3-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="533e3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="533e3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="533e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="533e3-116">Not supported.</span></span>    |
|<span data-ttu-id="533e3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="533e3-117">Application</span></span> | <span data-ttu-id="533e3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="533e3-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="533e3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="533e3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="533e3-120">Observe que ``<id>`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="533e3-120">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="533e3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="533e3-121">Request headers</span></span>
| <span data-ttu-id="533e3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="533e3-122">Name</span></span>       | <span data-ttu-id="533e3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="533e3-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="533e3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="533e3-124">Authorization</span></span>  | <span data-ttu-id="533e3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="533e3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="533e3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="533e3-127">Request body</span></span>
<span data-ttu-id="533e3-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="533e3-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="533e3-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="533e3-129">Parameter</span></span>    | <span data-ttu-id="533e3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="533e3-130">Type</span></span>   |<span data-ttu-id="533e3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="533e3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="533e3-132">motivos</span><span class="sxs-lookup"><span data-stu-id="533e3-132">reason</span></span>|<span data-ttu-id="533e3-133">string</span><span class="sxs-lookup"><span data-stu-id="533e3-133">string</span></span>|<span data-ttu-id="533e3-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="533e3-134">Optional.</span></span> <span data-ttu-id="533e3-135">Descrição sobre o motivo para esta ativação de função.</span><span class="sxs-lookup"><span data-stu-id="533e3-135">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="533e3-136">duration</span><span class="sxs-lookup"><span data-stu-id="533e3-136">duration</span></span>|<span data-ttu-id="533e3-137">string</span><span class="sxs-lookup"><span data-stu-id="533e3-137">string</span></span>|<span data-ttu-id="533e3-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="533e3-138">Optional.</span></span> <span data-ttu-id="533e3-139">Os valores válidos podem ```min``` ser (duração mínima da ativação ```default``` ), (duração de ativação padrão para a função) ou um valor duplo para especificar quantas horas é a ativação.</span><span class="sxs-lookup"><span data-stu-id="533e3-139">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="533e3-140">A duração especificada não pode ser maior do que a duração de ativação da função da configuração de função.</span><span class="sxs-lookup"><span data-stu-id="533e3-140">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="533e3-141">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="533e3-141">ticketNumber</span></span>|<span data-ttu-id="533e3-142">string</span><span class="sxs-lookup"><span data-stu-id="533e3-142">string</span></span>|<span data-ttu-id="533e3-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="533e3-143">Optional.</span></span> <span data-ttu-id="533e3-144">O número do tíquete usado para controlar esta ativação de função.</span><span class="sxs-lookup"><span data-stu-id="533e3-144">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="533e3-145">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="533e3-145">ticketSystem</span></span>|<span data-ttu-id="533e3-146">string</span><span class="sxs-lookup"><span data-stu-id="533e3-146">string</span></span>|<span data-ttu-id="533e3-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="533e3-147">Optional.</span></span> <span data-ttu-id="533e3-148">O sistema de permissão.</span><span class="sxs-lookup"><span data-stu-id="533e3-148">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="533e3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="533e3-149">Response</span></span>

<span data-ttu-id="533e3-150">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="533e3-150">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="533e3-151">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="533e3-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="533e3-152">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="533e3-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="533e3-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="533e3-153">Example</span></span>
<span data-ttu-id="533e3-154">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="533e3-154">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="533e3-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="533e3-155">Request</span></span>
<span data-ttu-id="533e3-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="533e3-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="533e3-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="533e3-157">Response</span></span>
<span data-ttu-id="533e3-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="533e3-158">Here is an example of the response.</span></span> 

><span data-ttu-id="533e3-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="533e3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="533e3-161">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="533e3-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="533e3-162">Basic</span><span class="sxs-lookup"><span data-stu-id="533e3-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/privilegedrole_selfactivate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="533e3-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="533e3-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/privilegedrole_selfactivate-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedrole-selfactivate.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedrole-selfactivate.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
