---
title: 'privilegedRoleAssignment: makeEligible'
description: Fazer a atribuição de função como qualificado. Se a atribuição de função já estiver elegível antes da chamada, ele não faz nada. Se a atribuição de função é permanente e o solicitante for diferente do usuário de destino, a atribuição de função se tornará qualificada e a função será desativada para o usuário de destino. Se o solicitante é o usuário de destino e a função é administrador de segurança ou administrador com privilégios de função, a função será ativada com a data de validade do padrão.
ms.openlocfilehash: f39f508c7aeae4d85db92b43f406cd3497533e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033775"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="cb01f-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="cb01f-106">privilegedRoleAssignment: makeEligible</span></span>

> <span data-ttu-id="cb01f-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cb01f-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb01f-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cb01f-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb01f-109">Fazer a atribuição de função como qualificado.</span><span class="sxs-lookup"><span data-stu-id="cb01f-109">Make the role assignment as eligible.</span></span> <span data-ttu-id="cb01f-110">Se a atribuição de função já estiver elegível antes da chamada, ele não faz nada.</span><span class="sxs-lookup"><span data-stu-id="cb01f-110">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="cb01f-111">Se a atribuição de função é permanente e o solicitante for diferente do usuário de destino, a atribuição de função se tornará qualificada e a função será desativada para o usuário de destino.</span><span class="sxs-lookup"><span data-stu-id="cb01f-111">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="cb01f-112">Se o solicitante é o usuário de destino e a função é administrador de segurança ou administrador com privilégios de função, a função será ativada com a data de validade do padrão.</span><span class="sxs-lookup"><span data-stu-id="cb01f-112">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb01f-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="cb01f-113">Permissions</span></span>
<span data-ttu-id="cb01f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb01f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cb01f-116">O solicitante precisa ter a função de _Administrador com privilégios de função_ .</span><span class="sxs-lookup"><span data-stu-id="cb01f-116">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="cb01f-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb01f-117">Permission type</span></span>      | <span data-ttu-id="cb01f-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb01f-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb01f-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb01f-119">Delegated (work or school account)</span></span> | <span data-ttu-id="cb01f-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb01f-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cb01f-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb01f-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb01f-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb01f-122">Not supported.</span></span>    |
|<span data-ttu-id="cb01f-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb01f-123">Application</span></span> | <span data-ttu-id="cb01f-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb01f-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb01f-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb01f-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="cb01f-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb01f-126">Request headers</span></span>
| <span data-ttu-id="cb01f-127">Nome</span><span class="sxs-lookup"><span data-stu-id="cb01f-127">Name</span></span>       | <span data-ttu-id="cb01f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb01f-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cb01f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb01f-129">Authorization</span></span>  | <span data-ttu-id="cb01f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb01f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb01f-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb01f-132">Request body</span></span>
<span data-ttu-id="cb01f-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb01f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb01f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb01f-134">Response</span></span>

<span data-ttu-id="cb01f-135">Se tiver êxito, este método retornará `200 OK` objeto response de código e [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb01f-135">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="cb01f-136">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="cb01f-136">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="cb01f-137">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="cb01f-137">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="cb01f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb01f-138">Example</span></span>
<span data-ttu-id="cb01f-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="cb01f-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cb01f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb01f-140">Request</span></span>
<span data-ttu-id="cb01f-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb01f-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```

##### <a name="response"></a><span data-ttu-id="cb01f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb01f-142">Response</span></span>
<span data-ttu-id="cb01f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb01f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->