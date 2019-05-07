---
title: Obter uma configuração de grupo
description: Recupere as propriedades de um objeto de configuração de grupo específico.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: aa78d40ae1d7434d5e0cba7fe9d8d117f8b8f900
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613288"
---
# <a name="get-a-group-setting"></a><span data-ttu-id="40dff-103">Obter uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="40dff-103">Get a group setting</span></span>

<span data-ttu-id="40dff-104">Recupere as propriedades de um objeto de configuração de grupo específico.</span><span class="sxs-lookup"><span data-stu-id="40dff-104">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40dff-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="40dff-105">Permissions</span></span>

<span data-ttu-id="40dff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40dff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="40dff-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40dff-108">Permission type</span></span>      | <span data-ttu-id="40dff-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40dff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40dff-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40dff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40dff-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40dff-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="40dff-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40dff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40dff-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40dff-113">Not supported.</span></span>    |
|<span data-ttu-id="40dff-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40dff-114">Application</span></span> | <span data-ttu-id="40dff-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40dff-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40dff-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40dff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="40dff-117">Obtenha uma configuração específica de todo o locatário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="40dff-117">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="40dff-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40dff-118">Optional query parameters</span></span>
<span data-ttu-id="40dff-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40dff-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="40dff-120">Observação: $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="40dff-120">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40dff-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40dff-121">Request headers</span></span>
| <span data-ttu-id="40dff-122">Nome</span><span class="sxs-lookup"><span data-stu-id="40dff-122">Name</span></span> | <span data-ttu-id="40dff-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="40dff-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="40dff-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="40dff-124">Authorization</span></span> | <span data-ttu-id="40dff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40dff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40dff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40dff-127">Request body</span></span>

<span data-ttu-id="40dff-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40dff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40dff-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="40dff-129">Response</span></span>

<span data-ttu-id="40dff-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40dff-130">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40dff-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40dff-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40dff-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40dff-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="40dff-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="40dff-133">Response</span></span>

<span data-ttu-id="40dff-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40dff-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="40dff-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="40dff-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="40dff-137">Basic</span><span class="sxs-lookup"><span data-stu-id="40dff-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_groupsetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40dff-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40dff-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_groupsetting-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsetting-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsetting-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
