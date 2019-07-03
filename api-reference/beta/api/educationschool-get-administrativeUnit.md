---
title: Obter administrativeUnit
description: Recupere o diretório simples **administrativeUnit** que corresponde a esse **educationSchool**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: d67782f07223391650040edfb306076d705699fd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441496"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="03830-103">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="03830-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03830-104">Recupere o diretório simples **administrativeUnit** que corresponde a esse **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="03830-104">Retrieve the simple directory **administrativeUnit** that corresponds to this **educationSchool**.</span></span>

><span data-ttu-id="03830-105">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="03830-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="03830-106">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="03830-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="03830-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="03830-107">Permissions</span></span>
<span data-ttu-id="03830-108">Uma combinação de permissões é obrigatória para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="03830-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="03830-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03830-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03830-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03830-110">Permission type</span></span>      | <span data-ttu-id="03830-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03830-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03830-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03830-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="03830-113">Uma de EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="03830-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="03830-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03830-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="03830-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03830-115">Not supported.</span></span>  |
|<span data-ttu-id="03830-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03830-116">Application</span></span> | <span data-ttu-id="03830-117">EduRoster.Read.All, EduRoster.ReadWrite.All além de Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="03830-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="03830-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03830-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/administrativeUnit
```
## <a name="request-headers"></a><span data-ttu-id="03830-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03830-119">Request headers</span></span>
| <span data-ttu-id="03830-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03830-120">Header</span></span>       | <span data-ttu-id="03830-121">Valor</span><span class="sxs-lookup"><span data-stu-id="03830-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="03830-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="03830-122">Authorization</span></span>  | <span data-ttu-id="03830-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03830-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03830-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03830-125">Request body</span></span>
<span data-ttu-id="03830-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03830-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="03830-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="03830-127">Response</span></span>
<span data-ttu-id="03830-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03830-128">If successful, this method returns a `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03830-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03830-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03830-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03830-130">Request</span></span>
<span data-ttu-id="03830-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="03830-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="03830-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="03830-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeUnit"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="03830-133">C#</span><span class="sxs-lookup"><span data-stu-id="03830-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="03830-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="03830-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="03830-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="03830-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="03830-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="03830-136">Response</span></span>
<span data-ttu-id="03830-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="03830-137">The following is an example of the response.</span></span> 

><span data-ttu-id="03830-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03830-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
