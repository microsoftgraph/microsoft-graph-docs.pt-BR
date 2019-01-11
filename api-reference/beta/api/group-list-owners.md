---
title: Listar proprietários
description: Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.
localization_priority: Normal
ms.openlocfilehash: d173b7a350d4aedbf1ec96b0b5e37da70e87d078
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878971"
---
# <a name="list-owners"></a><span data-ttu-id="7c57f-104">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="7c57f-104">List owners</span></span>

> <span data-ttu-id="7c57f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7c57f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c57f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7c57f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c57f-p103">Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="7c57f-p103">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c57f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c57f-109">Permissions</span></span>
<span data-ttu-id="7c57f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c57f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c57f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c57f-112">Permission type</span></span>      | <span data-ttu-id="7c57f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c57f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c57f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c57f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7c57f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c57f-115">Not supported.</span></span>    |
|<span data-ttu-id="7c57f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c57f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c57f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c57f-117">Not supported.</span></span>    |
|<span data-ttu-id="7c57f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c57f-118">Application</span></span> | <span data-ttu-id="7c57f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c57f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c57f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c57f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c57f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7c57f-121">Optional query parameters</span></span>
<span data-ttu-id="7c57f-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7c57f-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c57f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c57f-123">Request headers</span></span>
| <span data-ttu-id="7c57f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7c57f-124">Name</span></span>       | <span data-ttu-id="7c57f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c57f-125">Type</span></span> | <span data-ttu-id="7c57f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c57f-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7c57f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c57f-127">Authorization</span></span>  | <span data-ttu-id="7c57f-128">string</span><span class="sxs-lookup"><span data-stu-id="7c57f-128">string</span></span>  | <span data-ttu-id="7c57f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c57f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c57f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c57f-131">Request body</span></span>
<span data-ttu-id="7c57f-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c57f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c57f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c57f-133">Response</span></span>
<span data-ttu-id="7c57f-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c57f-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c57f-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c57f-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7c57f-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c57f-136">Request</span></span>
<span data-ttu-id="7c57f-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c57f-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="7c57f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c57f-138">Response</span></span>
<span data-ttu-id="7c57f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7c57f-139">The following is an example of the response.</span></span>
><span data-ttu-id="7c57f-140">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7c57f-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7c57f-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c57f-141">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
