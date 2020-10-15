---
title: Obter uma configuração de grupo
description: Recupere as propriedades de um objeto de configuração de grupo específico.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 10647c9c733ae684effdb1e9be5197cfca07bc0e
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460339"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="73698-103">Obter uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="73698-103">Get a group setting</span></span>

<span data-ttu-id="73698-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73698-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73698-105">Recupere as propriedades de um objeto de configuração de grupo específico.</span><span class="sxs-lookup"><span data-stu-id="73698-105">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73698-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="73698-106">Permissions</span></span>

<span data-ttu-id="73698-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73698-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="73698-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73698-109">Permission type</span></span>      | <span data-ttu-id="73698-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73698-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73698-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73698-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73698-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73698-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73698-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73698-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73698-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73698-114">Not supported.</span></span>    |
|<span data-ttu-id="73698-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73698-115">Application</span></span> | <span data-ttu-id="73698-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73698-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73698-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73698-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="73698-118">Obtenha uma configuração específica de todo o locatário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="73698-118">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="73698-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="73698-119">Optional query parameters</span></span>
<span data-ttu-id="73698-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="73698-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> <span data-ttu-id="73698-121">Observação: $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="73698-121">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73698-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73698-122">Request headers</span></span>
| <span data-ttu-id="73698-123">Nome</span><span class="sxs-lookup"><span data-stu-id="73698-123">Name</span></span> | <span data-ttu-id="73698-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="73698-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="73698-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="73698-125">Authorization</span></span> | <span data-ttu-id="73698-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73698-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73698-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73698-128">Request body</span></span>

<span data-ttu-id="73698-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73698-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73698-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="73698-130">Response</span></span>

<span data-ttu-id="73698-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73698-131">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73698-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73698-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73698-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73698-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="73698-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="73698-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="c"></a>[<span data-ttu-id="73698-135">C#</span><span class="sxs-lookup"><span data-stu-id="73698-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73698-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73698-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73698-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73698-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73698-138">Java</span><span class="sxs-lookup"><span data-stu-id="73698-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="73698-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="73698-139">Response</span></span>

<span data-ttu-id="73698-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73698-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
