---
title: 'privilegedRole: selfDeactivate'
description: Desative a função que é atribuída ao solicitante.
localization_priority: Normal
ms.openlocfilehash: 1cf76b59252516f75290c361d5c54e85895848cc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264215"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="18ef3-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="18ef3-103">privilegedRole: selfDeactivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18ef3-104">Desative a função que é atribuída ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="18ef3-104">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="18ef3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="18ef3-105">Permissions</span></span>
<span data-ttu-id="18ef3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="18ef3-108">O solicitante só pode chamar ```selfDeactivate``` a função que é atribuída a ele.</span><span class="sxs-lookup"><span data-stu-id="18ef3-108">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="18ef3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18ef3-109">Permission type</span></span>      | <span data-ttu-id="18ef3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18ef3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18ef3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18ef3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18ef3-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18ef3-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="18ef3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18ef3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18ef3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18ef3-114">Not supported.</span></span>    |
|<span data-ttu-id="18ef3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18ef3-115">Application</span></span> | <span data-ttu-id="18ef3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18ef3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18ef3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18ef3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="18ef3-118">Observe que ``<id>`` é a ID da função de destino.</span><span class="sxs-lookup"><span data-stu-id="18ef3-118">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="18ef3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18ef3-119">Request headers</span></span>
| <span data-ttu-id="18ef3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="18ef3-120">Name</span></span>       | <span data-ttu-id="18ef3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="18ef3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="18ef3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="18ef3-122">Authorization</span></span>  | <span data-ttu-id="18ef3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18ef3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18ef3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18ef3-125">Request body</span></span>
<span data-ttu-id="18ef3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18ef3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18ef3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="18ef3-127">Response</span></span>

<span data-ttu-id="18ef3-128">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18ef3-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="18ef3-129">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="18ef3-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="18ef3-130">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="18ef3-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="18ef3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18ef3-131">Example</span></span>
<span data-ttu-id="18ef3-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="18ef3-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18ef3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18ef3-133">Request</span></span>
<span data-ttu-id="18ef3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18ef3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="18ef3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="18ef3-135">Response</span></span>
<span data-ttu-id="18ef3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18ef3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="18ef3-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="18ef3-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="18ef3-140">C#</span><span class="sxs-lookup"><span data-stu-id="18ef3-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/privilegedrole_selfdeactivate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18ef3-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="18ef3-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/privilegedrole_selfdeactivate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="18ef3-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="18ef3-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/privilegedrole_selfdeactivate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-selfdeactivate.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedrole-selfdeactivate.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedrole-selfdeactivate.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
