---
title: 'privilegedRoleAssignment: makePermanent'
description: Torne a atribuição de função como permanente.
localization_priority: Normal
ms.openlocfilehash: 9c6334662cf8496262b49b14ceb3f51f7a4f8dbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538683"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="08e97-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="08e97-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08e97-104">Torne a atribuição de função como permanente.</span><span class="sxs-lookup"><span data-stu-id="08e97-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="08e97-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="08e97-105">Permissions</span></span>
<span data-ttu-id="08e97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08e97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="08e97-108">O locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="08e97-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="08e97-109">Caso contrário, o erro HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="08e97-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="08e97-110">O solicitante precisa ter função de _administrador de função privilegiada_ .</span><span class="sxs-lookup"><span data-stu-id="08e97-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="08e97-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08e97-111">Permission type</span></span>      | <span data-ttu-id="08e97-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08e97-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08e97-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08e97-113">Delegated (work or school account)</span></span> | <span data-ttu-id="08e97-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08e97-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="08e97-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08e97-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08e97-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08e97-116">Not supported.</span></span>    |
|<span data-ttu-id="08e97-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08e97-117">Application</span></span> | <span data-ttu-id="08e97-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08e97-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08e97-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08e97-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="08e97-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08e97-120">Request headers</span></span>
| <span data-ttu-id="08e97-121">Nome</span><span class="sxs-lookup"><span data-stu-id="08e97-121">Name</span></span>       | <span data-ttu-id="08e97-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="08e97-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="08e97-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="08e97-123">Authorization</span></span>  | <span data-ttu-id="08e97-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08e97-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08e97-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08e97-126">Request body</span></span>
<span data-ttu-id="08e97-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08e97-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08e97-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="08e97-128">Parameter</span></span>    | <span data-ttu-id="08e97-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="08e97-129">Type</span></span>   |<span data-ttu-id="08e97-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="08e97-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08e97-131">motivos</span><span class="sxs-lookup"><span data-stu-id="08e97-131">reason</span></span>|<span data-ttu-id="08e97-132">string</span><span class="sxs-lookup"><span data-stu-id="08e97-132">string</span></span>|<span data-ttu-id="08e97-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="08e97-133">Optional.</span></span> <span data-ttu-id="08e97-134">O motivo para fazer essa chamada.</span><span class="sxs-lookup"><span data-stu-id="08e97-134">The reason to make this call.</span></span>|
|<span data-ttu-id="08e97-135">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="08e97-135">ticketNumber</span></span>|<span data-ttu-id="08e97-136">string</span><span class="sxs-lookup"><span data-stu-id="08e97-136">string</span></span>|<span data-ttu-id="08e97-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="08e97-137">Optional.</span></span> <span data-ttu-id="08e97-138">O número do tíquete associado a esta ação.</span><span class="sxs-lookup"><span data-stu-id="08e97-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="08e97-139">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="08e97-139">ticketSystem</span></span>|<span data-ttu-id="08e97-140">string</span><span class="sxs-lookup"><span data-stu-id="08e97-140">string</span></span>|<span data-ttu-id="08e97-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="08e97-141">Optional.</span></span> <span data-ttu-id="08e97-142">O sistema de permissão.</span><span class="sxs-lookup"><span data-stu-id="08e97-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="08e97-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="08e97-143">Response</span></span>

<span data-ttu-id="08e97-144">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08e97-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08e97-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08e97-145">Example</span></span>
<span data-ttu-id="08e97-146">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="08e97-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="08e97-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08e97-147">Request</span></span>
<span data-ttu-id="08e97-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08e97-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="08e97-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="08e97-149">Response</span></span>
<span data-ttu-id="08e97-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08e97-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedroleassignment-makepermanent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
