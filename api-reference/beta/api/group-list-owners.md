---
title: Listar proprietários
description: Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 477a8fd2e647d8bdc3babdcb48bccba469912e93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520946"
---
# <a name="list-owners"></a><span data-ttu-id="8626a-104">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="8626a-104">List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8626a-p102">Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="8626a-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8626a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8626a-107">Permissions</span></span>
<span data-ttu-id="8626a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8626a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8626a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8626a-110">Permission type</span></span>      | <span data-ttu-id="8626a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8626a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8626a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8626a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8626a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8626a-113">Not supported.</span></span>    |
|<span data-ttu-id="8626a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8626a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8626a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8626a-115">Not supported.</span></span>    |
|<span data-ttu-id="8626a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8626a-116">Application</span></span> | <span data-ttu-id="8626a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8626a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8626a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8626a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8626a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8626a-119">Optional query parameters</span></span>
<span data-ttu-id="8626a-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8626a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8626a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8626a-121">Request headers</span></span>
| <span data-ttu-id="8626a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8626a-122">Name</span></span>       | <span data-ttu-id="8626a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8626a-123">Type</span></span> | <span data-ttu-id="8626a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8626a-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8626a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8626a-125">Authorization</span></span>  | <span data-ttu-id="8626a-126">string</span><span class="sxs-lookup"><span data-stu-id="8626a-126">string</span></span>  | <span data-ttu-id="8626a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8626a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8626a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8626a-129">Request body</span></span>
<span data-ttu-id="8626a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8626a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8626a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8626a-131">Response</span></span>
<span data-ttu-id="8626a-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8626a-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8626a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8626a-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8626a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8626a-134">Request</span></span>
<span data-ttu-id="8626a-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8626a-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="8626a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8626a-136">Response</span></span>
<span data-ttu-id="8626a-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8626a-137">The following is an example of the response.</span></span>
><span data-ttu-id="8626a-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8626a-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8626a-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8626a-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
