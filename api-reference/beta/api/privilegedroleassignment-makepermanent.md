---
title: 'privilegedRoleAssignment: makePermanent'
description: Fazer a atribuição de função como permanente.
ms.openlocfilehash: 06875fc62539598a5e1e806714fcae3d973ba29c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040828"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="33f48-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="33f48-103">privilegedRoleAssignment: makePermanent</span></span>

> <span data-ttu-id="33f48-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="33f48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33f48-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="33f48-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33f48-106">Fazer a atribuição de função como permanente.</span><span class="sxs-lookup"><span data-stu-id="33f48-106">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="33f48-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="33f48-107">Permissions</span></span>
<span data-ttu-id="33f48-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33f48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="33f48-110">O inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="33f48-110">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="33f48-111">Caso contrário, será retornado o erro de HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="33f48-111">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="33f48-112">O solicitante precisa ter a função de _Administrador com privilégios de função_ .</span><span class="sxs-lookup"><span data-stu-id="33f48-112">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="33f48-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33f48-113">Permission type</span></span>      | <span data-ttu-id="33f48-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33f48-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33f48-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33f48-115">Delegated (work or school account)</span></span> | <span data-ttu-id="33f48-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33f48-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33f48-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33f48-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33f48-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33f48-118">Not supported.</span></span>    |
|<span data-ttu-id="33f48-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33f48-119">Application</span></span> | <span data-ttu-id="33f48-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33f48-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="33f48-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33f48-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="33f48-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33f48-122">Request headers</span></span>
| <span data-ttu-id="33f48-123">Nome</span><span class="sxs-lookup"><span data-stu-id="33f48-123">Name</span></span>       | <span data-ttu-id="33f48-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="33f48-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="33f48-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="33f48-125">Authorization</span></span>  | <span data-ttu-id="33f48-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33f48-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33f48-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33f48-128">Request body</span></span>
<span data-ttu-id="33f48-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33f48-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="33f48-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="33f48-130">Parameter</span></span>    | <span data-ttu-id="33f48-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="33f48-131">Type</span></span>   |<span data-ttu-id="33f48-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="33f48-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33f48-133">motivo</span><span class="sxs-lookup"><span data-stu-id="33f48-133">reason</span></span>|<span data-ttu-id="33f48-134">string</span><span class="sxs-lookup"><span data-stu-id="33f48-134">string</span></span>|<span data-ttu-id="33f48-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33f48-135">Optional.</span></span> <span data-ttu-id="33f48-136">O motivo para fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="33f48-136">The reason to make this call.</span></span>|
|<span data-ttu-id="33f48-137">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="33f48-137">ticketNumber</span></span>|<span data-ttu-id="33f48-138">string</span><span class="sxs-lookup"><span data-stu-id="33f48-138">string</span></span>|<span data-ttu-id="33f48-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33f48-139">Optional.</span></span> <span data-ttu-id="33f48-140">O número de tíquete que é associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="33f48-140">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="33f48-141">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="33f48-141">ticketSystem</span></span>|<span data-ttu-id="33f48-142">string</span><span class="sxs-lookup"><span data-stu-id="33f48-142">string</span></span>|<span data-ttu-id="33f48-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33f48-143">Optional.</span></span> <span data-ttu-id="33f48-144">O sistema de tíquete.</span><span class="sxs-lookup"><span data-stu-id="33f48-144">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="33f48-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="33f48-145">Response</span></span>

<span data-ttu-id="33f48-146">Se tiver êxito, este método retornará `200 OK` objeto response de código e [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33f48-146">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33f48-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33f48-147">Example</span></span>
<span data-ttu-id="33f48-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="33f48-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="33f48-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33f48-149">Request</span></span>
<span data-ttu-id="33f48-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33f48-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="33f48-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="33f48-151">Response</span></span>
<span data-ttu-id="33f48-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33f48-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makePermanent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->