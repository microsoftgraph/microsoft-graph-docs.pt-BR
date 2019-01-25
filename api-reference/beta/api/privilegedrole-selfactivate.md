---
title: 'privilegedRole: selfActivate'
description: Ative a função que é atribuída ao solicitante.
localization_priority: Normal
ms.openlocfilehash: e0197599373246853906b879c0f3d13e61a45244
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515066"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="e1303-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="e1303-103">privilegedRole: selfActivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1303-104">Ative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="e1303-104">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="e1303-105">**Observação:** De 2018 efetivo de dezembro, essa API não será suportada e não deve ser usado.</span><span class="sxs-lookup"><span data-stu-id="e1303-105">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="e1303-106">Use o [PrivilegedRoleAssignmentRequest criar](privilegedroleassignmentrequest-post.md) .</span><span class="sxs-lookup"><span data-stu-id="e1303-106">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="e1303-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1303-107">Permissions</span></span>
<span data-ttu-id="e1303-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1303-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e1303-110">O solicitante só pode chamar ```selfActivate``` para a função que é atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="e1303-110">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="e1303-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1303-111">Permission type</span></span>      | <span data-ttu-id="e1303-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1303-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1303-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1303-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e1303-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1303-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e1303-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1303-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1303-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1303-116">Not supported.</span></span>    |
|<span data-ttu-id="e1303-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1303-117">Application</span></span> | <span data-ttu-id="e1303-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1303-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1303-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1303-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="e1303-120">Observe que ``<id>`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="e1303-120">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e1303-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1303-121">Request headers</span></span>
| <span data-ttu-id="e1303-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e1303-122">Name</span></span>       | <span data-ttu-id="e1303-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1303-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1303-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1303-124">Authorization</span></span>  | <span data-ttu-id="e1303-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1303-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1303-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1303-127">Request body</span></span>
<span data-ttu-id="e1303-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1303-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e1303-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e1303-129">Parameter</span></span>    | <span data-ttu-id="e1303-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1303-130">Type</span></span>   |<span data-ttu-id="e1303-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1303-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1303-132">Reason</span><span class="sxs-lookup"><span data-stu-id="e1303-132">reason</span></span>|<span data-ttu-id="e1303-133">string</span><span class="sxs-lookup"><span data-stu-id="e1303-133">string</span></span>|<span data-ttu-id="e1303-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e1303-134">Optional.</span></span> <span data-ttu-id="e1303-135">Descrição sobre o motivo de ativação essa função.</span><span class="sxs-lookup"><span data-stu-id="e1303-135">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="e1303-136">duration</span><span class="sxs-lookup"><span data-stu-id="e1303-136">duration</span></span>|<span data-ttu-id="e1303-137">string</span><span class="sxs-lookup"><span data-stu-id="e1303-137">string</span></span>|<span data-ttu-id="e1303-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e1303-138">Optional.</span></span> <span data-ttu-id="e1303-139">Valores válidos poderia ser ```min``` (duração mínima de ativação), ```default``` (duração de ativação padrão para a função,) ou um valor double para especificar quantas horas é a ativação.</span><span class="sxs-lookup"><span data-stu-id="e1303-139">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="e1303-140">A duração especificada não pode ser maior que a duração de ativação da função da configuração da função.</span><span class="sxs-lookup"><span data-stu-id="e1303-140">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="e1303-141">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="e1303-141">ticketNumber</span></span>|<span data-ttu-id="e1303-142">string</span><span class="sxs-lookup"><span data-stu-id="e1303-142">string</span></span>|<span data-ttu-id="e1303-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e1303-143">Optional.</span></span> <span data-ttu-id="e1303-144">O número de tíquete que é usado para acompanhamento ativação essa função.</span><span class="sxs-lookup"><span data-stu-id="e1303-144">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="e1303-145">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="e1303-145">ticketSystem</span></span>|<span data-ttu-id="e1303-146">string</span><span class="sxs-lookup"><span data-stu-id="e1303-146">string</span></span>|<span data-ttu-id="e1303-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e1303-147">Optional.</span></span> <span data-ttu-id="e1303-148">O sistema de tíquete.</span><span class="sxs-lookup"><span data-stu-id="e1303-148">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="e1303-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1303-149">Response</span></span>

<span data-ttu-id="e1303-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1303-150">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="e1303-151">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="e1303-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="e1303-152">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="e1303-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="e1303-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1303-153">Example</span></span>
<span data-ttu-id="e1303-154">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e1303-154">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e1303-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1303-155">Request</span></span>
<span data-ttu-id="e1303-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1303-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e1303-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1303-157">Response</span></span>
<span data-ttu-id="e1303-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1303-158">Here is an example of the response.</span></span> 

><span data-ttu-id="e1303-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1303-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedrole-selfactivate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
