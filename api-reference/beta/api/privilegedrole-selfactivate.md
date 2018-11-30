---
title: 'privilegedRole: selfActivate'
description: Ative a função que é atribuída ao solicitante.
ms.openlocfilehash: bff445bf1fa5d7c0dfbce080b4361b0479b7dcb7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039162"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="6e2fc-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="6e2fc-103">privilegedRole: selfActivate</span></span>

><span data-ttu-id="6e2fc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e2fc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e2fc-106">Ative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-106">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="6e2fc-107">**Observação:** De 2018 efetivo de dezembro, essa API não será suportada e não deve ser usado.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-107">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="6e2fc-108">Use o [PrivilegedRoleAssignmentRequest criar](privilegedroleassignmentrequest-post.md) .</span><span class="sxs-lookup"><span data-stu-id="6e2fc-108">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="6e2fc-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="6e2fc-109">Permissions</span></span>
<span data-ttu-id="6e2fc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e2fc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6e2fc-112">O solicitante só pode chamar ```selfActivate``` para a função que é atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-112">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="6e2fc-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e2fc-113">Permission type</span></span>      | <span data-ttu-id="6e2fc-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e2fc-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e2fc-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e2fc-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6e2fc-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6e2fc-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6e2fc-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e2fc-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e2fc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-118">Not supported.</span></span>    |
|<span data-ttu-id="6e2fc-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e2fc-119">Application</span></span> | <span data-ttu-id="6e2fc-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e2fc-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e2fc-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="6e2fc-122">Observe que ``<id>`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-122">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6e2fc-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e2fc-123">Request headers</span></span>
| <span data-ttu-id="6e2fc-124">Nome</span><span class="sxs-lookup"><span data-stu-id="6e2fc-124">Name</span></span>       | <span data-ttu-id="6e2fc-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e2fc-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6e2fc-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e2fc-126">Authorization</span></span>  | <span data-ttu-id="6e2fc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e2fc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e2fc-129">Request body</span></span>
<span data-ttu-id="6e2fc-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6e2fc-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6e2fc-131">Parameter</span></span>    | <span data-ttu-id="6e2fc-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e2fc-132">Type</span></span>   |<span data-ttu-id="6e2fc-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e2fc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e2fc-134">motivo</span><span class="sxs-lookup"><span data-stu-id="6e2fc-134">reason</span></span>|<span data-ttu-id="6e2fc-135">string</span><span class="sxs-lookup"><span data-stu-id="6e2fc-135">string</span></span>|<span data-ttu-id="6e2fc-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-136">Optional.</span></span> <span data-ttu-id="6e2fc-137">Descrição sobre o motivo de ativação essa função.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-137">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="6e2fc-138">duration</span><span class="sxs-lookup"><span data-stu-id="6e2fc-138">duration</span></span>|<span data-ttu-id="6e2fc-139">string</span><span class="sxs-lookup"><span data-stu-id="6e2fc-139">string</span></span>|<span data-ttu-id="6e2fc-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-140">Optional.</span></span> <span data-ttu-id="6e2fc-141">Valores válidos poderia ser ```min``` (duração mínima de ativação), ```default``` (duração de ativação padrão para a função,) ou um valor double para especificar quantas horas é a ativação.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-141">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="6e2fc-142">A duração especificada não pode ser maior que a duração de ativação da função da configuração da função.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-142">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="6e2fc-143">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="6e2fc-143">ticketNumber</span></span>|<span data-ttu-id="6e2fc-144">string</span><span class="sxs-lookup"><span data-stu-id="6e2fc-144">string</span></span>|<span data-ttu-id="6e2fc-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-145">Optional.</span></span> <span data-ttu-id="6e2fc-146">O número de tíquete que é usado para acompanhamento ativação essa função.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-146">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="6e2fc-147">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="6e2fc-147">ticketSystem</span></span>|<span data-ttu-id="6e2fc-148">string</span><span class="sxs-lookup"><span data-stu-id="6e2fc-148">string</span></span>|<span data-ttu-id="6e2fc-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-149">Optional.</span></span> <span data-ttu-id="6e2fc-150">O sistema de tíquete.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-150">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="6e2fc-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e2fc-151">Response</span></span>

<span data-ttu-id="6e2fc-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-152">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="6e2fc-153">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-153">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6e2fc-154">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-154">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="6e2fc-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e2fc-155">Example</span></span>
<span data-ttu-id="6e2fc-156">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-156">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6e2fc-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e2fc-157">Request</span></span>
<span data-ttu-id="6e2fc-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6e2fc-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e2fc-159">Response</span></span>
<span data-ttu-id="6e2fc-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-160">Here is an example of the response.</span></span> 

><span data-ttu-id="6e2fc-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e2fc-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
