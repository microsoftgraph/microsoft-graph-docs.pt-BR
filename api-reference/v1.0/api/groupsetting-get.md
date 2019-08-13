---
title: Obter uma configuração de grupo
description: Recupere as propriedades de um objeto de configuração de grupo específico.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c577e327534c6c96637a27f74edb40fb0b0a3cf0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373298"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="5471b-103">Obter uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="5471b-103">Get a group setting</span></span>

<span data-ttu-id="5471b-104">Recupere as propriedades de um objeto de configuração de grupo específico.</span><span class="sxs-lookup"><span data-stu-id="5471b-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5471b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5471b-105">Permissions</span></span>

<span data-ttu-id="5471b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5471b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5471b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5471b-108">Permission type</span></span>      | <span data-ttu-id="5471b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5471b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5471b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5471b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5471b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5471b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5471b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5471b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5471b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5471b-113">Not supported.</span></span>    |
|<span data-ttu-id="5471b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5471b-114">Application</span></span> | <span data-ttu-id="5471b-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5471b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5471b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5471b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="5471b-117">Obtenha uma configuração específica de todo o locatário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="5471b-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5471b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5471b-118">Optional query parameters</span></span>
<span data-ttu-id="5471b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5471b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="5471b-120">Observação: $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="5471b-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5471b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5471b-121">Request headers</span></span>
| <span data-ttu-id="5471b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5471b-122">Name</span></span> | <span data-ttu-id="5471b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5471b-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="5471b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5471b-124">Authorization</span></span> | <span data-ttu-id="5471b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5471b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5471b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5471b-127">Request body</span></span>

<span data-ttu-id="5471b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5471b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5471b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5471b-129">Response</span></span>

<span data-ttu-id="5471b-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5471b-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5471b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5471b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5471b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5471b-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5471b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5471b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5471b-134">C#</span><span class="sxs-lookup"><span data-stu-id="5471b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5471b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5471b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5471b-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5471b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5471b-137">Java</span><span class="sxs-lookup"><span data-stu-id="5471b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5471b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5471b-138">Response</span></span>

<span data-ttu-id="5471b-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5471b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
