---
title: 'privilegedRoleAssignment: My'
description: Obtenha as atribuições de função privilegiada do solicitante.
localization_priority: Normal
ms.openlocfilehash: acf03e62eff3195fb922a324a231e5d58f768b11
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337310"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="bb5a3-103">privilegedRoleAssignment: My</span><span class="sxs-lookup"><span data-stu-id="bb5a3-103">privilegedRoleAssignment: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb5a3-104">Obtenha as atribuições de função privilegiada do solicitante.</span><span class="sxs-lookup"><span data-stu-id="bb5a3-104">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb5a3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb5a3-105">Permissions</span></span>
<span data-ttu-id="bb5a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb5a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb5a3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb5a3-108">Permission type</span></span>      | <span data-ttu-id="bb5a3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb5a3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb5a3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb5a3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bb5a3-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb5a3-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bb5a3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb5a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb5a3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb5a3-113">Not supported.</span></span>    |
|<span data-ttu-id="bb5a3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb5a3-114">Application</span></span> | <span data-ttu-id="bb5a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb5a3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb5a3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb5a3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="bb5a3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5a3-117">Request headers</span></span>
| <span data-ttu-id="bb5a3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bb5a3-118">Name</span></span>       | <span data-ttu-id="bb5a3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb5a3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bb5a3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb5a3-120">Authorization</span></span>  | <span data-ttu-id="bb5a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb5a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb5a3-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5a3-123">Request body</span></span>
<span data-ttu-id="bb5a3-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb5a3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb5a3-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb5a3-125">Response</span></span>

<span data-ttu-id="bb5a3-126">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto da coleção [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb5a3-126">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb5a3-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb5a3-127">Example</span></span>
<span data-ttu-id="bb5a3-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bb5a3-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bb5a3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5a3-129">Request</span></span>
<span data-ttu-id="bb5a3-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb5a3-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="bb5a3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb5a3-131">Response</span></span>
<span data-ttu-id="bb5a3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb5a3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
