---
title: Obter uma configuração de grupo
description: Recupere as propriedades de um objeto de configuração de grupo específico.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b7e8d6839606519e3bfe772b14068184d2b1947d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051414"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="44b01-103">Obter uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="44b01-103">Get a group setting</span></span>

<span data-ttu-id="44b01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44b01-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44b01-105">Recupere as propriedades de um objeto de configuração de grupo específico.</span><span class="sxs-lookup"><span data-stu-id="44b01-105">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44b01-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="44b01-106">Permissions</span></span>

<span data-ttu-id="44b01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44b01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="44b01-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44b01-109">Permission type</span></span>      | <span data-ttu-id="44b01-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44b01-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44b01-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44b01-111">Delegated (work or school account)</span></span> | <span data-ttu-id="44b01-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="44b01-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="44b01-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44b01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44b01-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44b01-114">Not supported.</span></span>    |
|<span data-ttu-id="44b01-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44b01-115">Application</span></span> | <span data-ttu-id="44b01-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44b01-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44b01-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44b01-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="44b01-118">Obter uma configuração específica de locatário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="44b01-118">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="44b01-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="44b01-119">Optional query parameters</span></span>
<span data-ttu-id="44b01-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="44b01-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> <span data-ttu-id="44b01-121">Observação: $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="44b01-121">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44b01-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44b01-122">Request headers</span></span>
| <span data-ttu-id="44b01-123">Nome</span><span class="sxs-lookup"><span data-stu-id="44b01-123">Name</span></span> | <span data-ttu-id="44b01-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="44b01-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="44b01-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="44b01-125">Authorization</span></span> | <span data-ttu-id="44b01-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44b01-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44b01-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44b01-128">Request body</span></span>

<span data-ttu-id="44b01-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="44b01-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44b01-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="44b01-130">Response</span></span>

<span data-ttu-id="44b01-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44b01-131">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44b01-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44b01-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44b01-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44b01-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="44b01-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="44b01-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="c"></a>[<span data-ttu-id="44b01-135">C#</span><span class="sxs-lookup"><span data-stu-id="44b01-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44b01-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44b01-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44b01-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44b01-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44b01-138">Java</span><span class="sxs-lookup"><span data-stu-id="44b01-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="44b01-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="44b01-139">Response</span></span>

<span data-ttu-id="44b01-140">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="44b01-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
