---
title: 'privilegedRoleAssignment: makeEligible'
description: Tornar a atribuição de função como qualificada. Se a atribuição de função já estiver qualificada antes da chamada, ela não fará nada. Se a atribuição de função for permanente e o solicitante for diferente do usuário de destino, a atribuição de função ficará qualificada e a função será desativada para o usuário de destino. Se o solicitante for o usuário de destino e a função for administrador de segurança ou administrador de função privilegiada, a função será ativada com a expiração padrão.
localization_priority: Normal
ms.openlocfilehash: 0cc2b650e90064dd18e66ede1a59c50dc23665e2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875689"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="24877-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="24877-106">privilegedRoleAssignment: makeEligible</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24877-107">Tornar a atribuição de função como qualificada.</span><span class="sxs-lookup"><span data-stu-id="24877-107">Make the role assignment as eligible.</span></span> <span data-ttu-id="24877-108">Se a atribuição de função já estiver qualificada antes da chamada, ela não fará nada.</span><span class="sxs-lookup"><span data-stu-id="24877-108">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="24877-109">Se a atribuição de função for permanente e o solicitante for diferente do usuário de destino, a atribuição de função ficará qualificada e a função será desativada para o usuário de destino.</span><span class="sxs-lookup"><span data-stu-id="24877-109">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="24877-110">Se o solicitante for o usuário de destino e a função for administrador de segurança ou administrador de função privilegiada, a função será ativada com a expiração padrão.</span><span class="sxs-lookup"><span data-stu-id="24877-110">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="24877-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="24877-111">Permissions</span></span>
<span data-ttu-id="24877-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24877-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="24877-114">O solicitante precisa ter função de _administrador de função privilegiada_ .</span><span class="sxs-lookup"><span data-stu-id="24877-114">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="24877-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24877-115">Permission type</span></span>      | <span data-ttu-id="24877-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24877-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24877-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24877-117">Delegated (work or school account)</span></span> | <span data-ttu-id="24877-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="24877-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="24877-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24877-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24877-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24877-120">Not supported.</span></span>    |
|<span data-ttu-id="24877-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24877-121">Application</span></span> | <span data-ttu-id="24877-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24877-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24877-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24877-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="24877-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24877-124">Request headers</span></span>
| <span data-ttu-id="24877-125">Nome</span><span class="sxs-lookup"><span data-stu-id="24877-125">Name</span></span>       | <span data-ttu-id="24877-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="24877-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="24877-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="24877-127">Authorization</span></span>  | <span data-ttu-id="24877-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24877-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24877-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24877-130">Request body</span></span>
<span data-ttu-id="24877-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24877-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24877-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="24877-132">Response</span></span>

<span data-ttu-id="24877-133">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24877-133">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="24877-134">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="24877-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="24877-135">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="24877-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="24877-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24877-136">Example</span></span>
<span data-ttu-id="24877-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="24877-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24877-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24877-138">Request</span></span>
<span data-ttu-id="24877-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24877-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="24877-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="24877-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="24877-141">C#</span><span class="sxs-lookup"><span data-stu-id="24877-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makeeligible-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24877-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="24877-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makeeligible-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="24877-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="24877-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makeeligible-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="24877-144">Java</span><span class="sxs-lookup"><span data-stu-id="24877-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makeeligible-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="24877-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="24877-145">Response</span></span>
<span data-ttu-id="24877-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24877-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
