---
title: 'privilegedRoleAssignment: makeEligible'
description: Tornar a atribuição de função como qualificada. Se a atribuição de função já estiver qualificada antes da chamada, ela não fará nada. Se a atribuição de função for permanente e o solicitante for diferente do usuário de destino, a atribuição de função ficará qualificada e a função será desativada para o usuário de destino. Se o solicitante for o usuário de destino e a função for administrador de segurança ou administrador de função privilegiada, a função será ativada com a expiração padrão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 93c7dbf415affaa64226000a2a01034821da74af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455344"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="dbdfc-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="dbdfc-106">privilegedRoleAssignment: makeEligible</span></span>

<span data-ttu-id="dbdfc-107">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dbdfc-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbdfc-108">Tornar a atribuição de função como qualificada.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-108">Make the role assignment as eligible.</span></span> <span data-ttu-id="dbdfc-109">Se a atribuição de função já estiver qualificada antes da chamada, ela não fará nada.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-109">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="dbdfc-110">Se a atribuição de função for permanente e o solicitante for diferente do usuário de destino, a atribuição de função ficará qualificada e a função será desativada para o usuário de destino.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-110">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="dbdfc-111">Se o solicitante for o usuário de destino e a função for administrador de segurança ou administrador de função privilegiada, a função será ativada com a expiração padrão.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-111">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbdfc-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbdfc-112">Permissions</span></span>
<span data-ttu-id="dbdfc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbdfc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dbdfc-115">O solicitante precisa ter função de _administrador de função privilegiada_ .</span><span class="sxs-lookup"><span data-stu-id="dbdfc-115">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="dbdfc-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbdfc-116">Permission type</span></span>      | <span data-ttu-id="dbdfc-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbdfc-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbdfc-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbdfc-118">Delegated (work or school account)</span></span> | <span data-ttu-id="dbdfc-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dbdfc-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dbdfc-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbdfc-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbdfc-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-121">Not supported.</span></span>    |
|<span data-ttu-id="dbdfc-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbdfc-122">Application</span></span> | <span data-ttu-id="dbdfc-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbdfc-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbdfc-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="dbdfc-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbdfc-125">Request headers</span></span>
| <span data-ttu-id="dbdfc-126">Nome</span><span class="sxs-lookup"><span data-stu-id="dbdfc-126">Name</span></span>       | <span data-ttu-id="dbdfc-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbdfc-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dbdfc-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbdfc-128">Authorization</span></span>  | <span data-ttu-id="dbdfc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbdfc-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbdfc-131">Request body</span></span>
<span data-ttu-id="dbdfc-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbdfc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbdfc-133">Response</span></span>

<span data-ttu-id="dbdfc-134">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-134">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="dbdfc-135">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-135">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="dbdfc-136">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-136">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="dbdfc-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbdfc-137">Example</span></span>
<span data-ttu-id="dbdfc-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dbdfc-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbdfc-139">Request</span></span>
<span data-ttu-id="dbdfc-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dbdfc-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbdfc-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```
# <a name="c"></a>[<span data-ttu-id="dbdfc-142">C#</span><span class="sxs-lookup"><span data-stu-id="dbdfc-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makeeligible-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dbdfc-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbdfc-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makeeligible-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dbdfc-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dbdfc-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makeeligible-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dbdfc-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbdfc-145">Response</span></span>
<span data-ttu-id="dbdfc-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbdfc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
