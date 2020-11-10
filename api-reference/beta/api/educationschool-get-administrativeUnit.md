---
title: Obter administrativeUnit
description: Recupere o diretório simples **administrativeUnit** que corresponde a esse **educationSchool**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 109f5a014674ee143305469e06c6b2af60592f19
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955607"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="c2780-103">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c2780-103">Get administrativeUnit</span></span>

<span data-ttu-id="c2780-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2780-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2780-105">Recupere o diretório simples **administrativeUnit** que corresponde a esse **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="c2780-105">Retrieve the simple directory **administrativeUnit** that corresponds to this **educationSchool**.</span></span>

><span data-ttu-id="c2780-106">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="c2780-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="c2780-107">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="c2780-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2780-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2780-108">Permissions</span></span>
<span data-ttu-id="c2780-109">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c2780-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="c2780-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2780-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2780-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2780-111">Permission type</span></span>      | <span data-ttu-id="c2780-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2780-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2780-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2780-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c2780-114">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2780-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="c2780-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2780-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c2780-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2780-116">Not supported.</span></span>  |
|<span data-ttu-id="c2780-117">Application</span><span class="sxs-lookup"><span data-stu-id="c2780-117">Application</span></span> | <span data-ttu-id="c2780-118">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2780-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="c2780-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2780-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/administrativeUnit
```
## <a name="request-headers"></a><span data-ttu-id="c2780-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2780-120">Request headers</span></span>
| <span data-ttu-id="c2780-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c2780-121">Header</span></span>       | <span data-ttu-id="c2780-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c2780-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c2780-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2780-123">Authorization</span></span>  | <span data-ttu-id="c2780-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2780-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2780-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2780-126">Request body</span></span>
<span data-ttu-id="c2780-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2780-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c2780-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2780-128">Response</span></span>
<span data-ttu-id="c2780-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2780-129">If successful, this method returns a `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2780-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2780-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2780-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2780-131">Request</span></span>
<span data-ttu-id="c2780-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2780-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2780-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2780-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_administrativeUnit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit
```
# <a name="c"></a>[<span data-ttu-id="c2780-134">C#</span><span class="sxs-lookup"><span data-stu-id="c2780-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2780-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2780-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2780-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2780-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2780-137">Java</span><span class="sxs-lookup"><span data-stu-id="c2780-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-get-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c2780-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2780-138">Response</span></span>
<span data-ttu-id="c2780-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c2780-139">The following is an example of the response.</span></span> 

><span data-ttu-id="c2780-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2780-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

<!-- uuid: A681726F-B4A7-4BCF-9407-F87CB9A4771D
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


