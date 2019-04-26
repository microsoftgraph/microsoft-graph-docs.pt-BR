---
title: 'privilegedRoleAssignment: makeEligible'
description: Tornar a atribuição de função como qualificada. Se a atribuição de função já estiver qualificada antes da chamada, ela não fará nada. Se a atribuição de função for permanente e o solicitante for diferente do usuário de destino, a atribuição de função ficará qualificada e a função será desativada para o usuário de destino. Se o solicitante for o usuário de destino e a função for administrador de segurança ou administrador de função privilegiada, a função será ativada com a expiração padrão.
localization_priority: Normal
ms.openlocfilehash: 6d3e6e58119a7a757da65d08eeeb97247a78d714
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337142"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="8de48-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="8de48-106">privilegedRoleAssignment: makeEligible</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8de48-107">Tornar a atribuição de função como qualificada.</span><span class="sxs-lookup"><span data-stu-id="8de48-107">Make the role assignment as eligible.</span></span> <span data-ttu-id="8de48-108">Se a atribuição de função já estiver qualificada antes da chamada, ela não fará nada.</span><span class="sxs-lookup"><span data-stu-id="8de48-108">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="8de48-109">Se a atribuição de função for permanente e o solicitante for diferente do usuário de destino, a atribuição de função ficará qualificada e a função será desativada para o usuário de destino.</span><span class="sxs-lookup"><span data-stu-id="8de48-109">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="8de48-110">Se o solicitante for o usuário de destino e a função for administrador de segurança ou administrador de função privilegiada, a função será ativada com a expiração padrão.</span><span class="sxs-lookup"><span data-stu-id="8de48-110">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="8de48-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="8de48-111">Permissions</span></span>
<span data-ttu-id="8de48-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8de48-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8de48-114">O solicitante precisa ter função de _administrador de função privilegiada_ .</span><span class="sxs-lookup"><span data-stu-id="8de48-114">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="8de48-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8de48-115">Permission type</span></span>      | <span data-ttu-id="8de48-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8de48-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8de48-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8de48-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8de48-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8de48-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8de48-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8de48-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8de48-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8de48-120">Not supported.</span></span>    |
|<span data-ttu-id="8de48-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8de48-121">Application</span></span> | <span data-ttu-id="8de48-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8de48-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8de48-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8de48-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="8de48-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8de48-124">Request headers</span></span>
| <span data-ttu-id="8de48-125">Nome</span><span class="sxs-lookup"><span data-stu-id="8de48-125">Name</span></span>       | <span data-ttu-id="8de48-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="8de48-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8de48-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="8de48-127">Authorization</span></span>  | <span data-ttu-id="8de48-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8de48-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8de48-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8de48-130">Request body</span></span>
<span data-ttu-id="8de48-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8de48-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8de48-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8de48-132">Response</span></span>

<span data-ttu-id="8de48-133">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8de48-133">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="8de48-134">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="8de48-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8de48-135">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="8de48-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="8de48-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8de48-136">Example</span></span>
<span data-ttu-id="8de48-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8de48-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8de48-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8de48-138">Request</span></span>
<span data-ttu-id="8de48-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8de48-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```

##### <a name="response"></a><span data-ttu-id="8de48-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8de48-140">Response</span></span>
<span data-ttu-id="8de48-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8de48-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
