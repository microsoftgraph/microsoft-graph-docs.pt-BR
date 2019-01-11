---
title: 'privilegedRole: selfActivate'
description: Ative a função que é atribuída ao solicitante.
localization_priority: Normal
ms.openlocfilehash: 9423d87714fcd4a7b7cce1dd5cd03bcef3e0ef9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872125"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="87c73-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="87c73-103">privilegedRole: selfActivate</span></span>

><span data-ttu-id="87c73-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="87c73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87c73-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87c73-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87c73-106">Ative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="87c73-106">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="87c73-107">**Observação:** De 2018 efetivo de dezembro, essa API não será suportada e não deve ser usado.</span><span class="sxs-lookup"><span data-stu-id="87c73-107">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="87c73-108">Use o [PrivilegedRoleAssignmentRequest criar](privilegedroleassignmentrequest-post.md) .</span><span class="sxs-lookup"><span data-stu-id="87c73-108">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="87c73-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="87c73-109">Permissions</span></span>
<span data-ttu-id="87c73-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87c73-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="87c73-112">O solicitante só pode chamar ```selfActivate``` para a função que é atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="87c73-112">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="87c73-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87c73-113">Permission type</span></span>      | <span data-ttu-id="87c73-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87c73-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87c73-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87c73-115">Delegated (work or school account)</span></span> | <span data-ttu-id="87c73-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="87c73-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="87c73-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87c73-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87c73-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87c73-118">Not supported.</span></span>    |
|<span data-ttu-id="87c73-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87c73-119">Application</span></span> | <span data-ttu-id="87c73-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87c73-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87c73-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87c73-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="87c73-122">Observe que ``<id>`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="87c73-122">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="87c73-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87c73-123">Request headers</span></span>
| <span data-ttu-id="87c73-124">Nome</span><span class="sxs-lookup"><span data-stu-id="87c73-124">Name</span></span>       | <span data-ttu-id="87c73-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="87c73-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="87c73-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="87c73-126">Authorization</span></span>  | <span data-ttu-id="87c73-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87c73-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87c73-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87c73-129">Request body</span></span>
<span data-ttu-id="87c73-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87c73-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="87c73-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="87c73-131">Parameter</span></span>    | <span data-ttu-id="87c73-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="87c73-132">Type</span></span>   |<span data-ttu-id="87c73-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="87c73-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87c73-134">motivo</span><span class="sxs-lookup"><span data-stu-id="87c73-134">reason</span></span>|<span data-ttu-id="87c73-135">string</span><span class="sxs-lookup"><span data-stu-id="87c73-135">string</span></span>|<span data-ttu-id="87c73-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="87c73-136">Optional.</span></span> <span data-ttu-id="87c73-137">Descrição sobre o motivo de ativação essa função.</span><span class="sxs-lookup"><span data-stu-id="87c73-137">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="87c73-138">duration</span><span class="sxs-lookup"><span data-stu-id="87c73-138">duration</span></span>|<span data-ttu-id="87c73-139">string</span><span class="sxs-lookup"><span data-stu-id="87c73-139">string</span></span>|<span data-ttu-id="87c73-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="87c73-140">Optional.</span></span> <span data-ttu-id="87c73-141">Valores válidos poderia ser ```min``` (duração mínima de ativação), ```default``` (duração de ativação padrão para a função,) ou um valor double para especificar quantas horas é a ativação.</span><span class="sxs-lookup"><span data-stu-id="87c73-141">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="87c73-142">A duração especificada não pode ser maior que a duração de ativação da função da configuração da função.</span><span class="sxs-lookup"><span data-stu-id="87c73-142">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="87c73-143">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="87c73-143">ticketNumber</span></span>|<span data-ttu-id="87c73-144">string</span><span class="sxs-lookup"><span data-stu-id="87c73-144">string</span></span>|<span data-ttu-id="87c73-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="87c73-145">Optional.</span></span> <span data-ttu-id="87c73-146">O número de tíquete que é usado para acompanhamento ativação essa função.</span><span class="sxs-lookup"><span data-stu-id="87c73-146">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="87c73-147">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="87c73-147">ticketSystem</span></span>|<span data-ttu-id="87c73-148">string</span><span class="sxs-lookup"><span data-stu-id="87c73-148">string</span></span>|<span data-ttu-id="87c73-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="87c73-149">Optional.</span></span> <span data-ttu-id="87c73-150">O sistema de tíquete.</span><span class="sxs-lookup"><span data-stu-id="87c73-150">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="87c73-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="87c73-151">Response</span></span>

<span data-ttu-id="87c73-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87c73-152">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="87c73-153">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="87c73-153">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="87c73-154">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="87c73-154">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="87c73-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87c73-155">Example</span></span>
<span data-ttu-id="87c73-156">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="87c73-156">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87c73-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87c73-157">Request</span></span>
<span data-ttu-id="87c73-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87c73-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="87c73-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="87c73-159">Response</span></span>
<span data-ttu-id="87c73-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87c73-160">Here is an example of the response.</span></span> 

><span data-ttu-id="87c73-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87c73-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
