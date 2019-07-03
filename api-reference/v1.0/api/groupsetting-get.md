---
title: Obter uma configuração de grupo
description: Recupere as propriedades de um objeto de configuração de grupo específico.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef401733d328b94f762c967a9a899dc95fdd79f1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447422"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="9bf3e-103">Obter uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="9bf3e-103">Get a group setting</span></span>

<span data-ttu-id="9bf3e-104">Recupere as propriedades de um objeto de configuração de grupo específico.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bf3e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9bf3e-105">Permissions</span></span>

<span data-ttu-id="9bf3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bf3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9bf3e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bf3e-108">Permission type</span></span>      | <span data-ttu-id="9bf3e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bf3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bf3e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bf3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9bf3e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9bf3e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9bf3e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bf3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bf3e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-113">Not supported.</span></span>    |
|<span data-ttu-id="9bf3e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bf3e-114">Application</span></span> | <span data-ttu-id="9bf3e-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bf3e-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bf3e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bf3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="9bf3e-117">Obtenha uma configuração específica de todo o locatário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9bf3e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9bf3e-118">Optional query parameters</span></span>
<span data-ttu-id="9bf3e-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="9bf3e-120">Observação: $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bf3e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf3e-121">Request headers</span></span>
| <span data-ttu-id="9bf3e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9bf3e-122">Name</span></span> | <span data-ttu-id="9bf3e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bf3e-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="9bf3e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bf3e-124">Authorization</span></span> | <span data-ttu-id="9bf3e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bf3e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf3e-127">Request body</span></span>

<span data-ttu-id="9bf3e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bf3e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf3e-129">Response</span></span>

<span data-ttu-id="9bf3e-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bf3e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bf3e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9bf3e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bf3e-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9bf3e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bf3e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9bf3e-134">C#</span><span class="sxs-lookup"><span data-stu-id="9bf3e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9bf3e-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="9bf3e-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9bf3e-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9bf3e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9bf3e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bf3e-137">Response</span></span>

<span data-ttu-id="9bf3e-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
