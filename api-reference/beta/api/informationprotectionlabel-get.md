---
title: Obter informationProtectionLabel
description: Recupere as propriedades e os relacionamentos do objeto informationProtectionLabel especificado.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9c4b923279004c91b3e9d4e185d87f9ee15457ed
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216677"
---
# <a name="get-informationprotectionlabel"></a><span data-ttu-id="43910-103">Obter informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="43910-103">Get informationProtectionLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43910-104">Recupere as propriedades e os relacionamentos de um objeto [informationProtectionLabel](../resources/informationprotectionlabel.md) .</span><span class="sxs-lookup"><span data-stu-id="43910-104">Retrieve the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="43910-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="43910-105">Permissions</span></span>

<span data-ttu-id="43910-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43910-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43910-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43910-108">Permission type</span></span>                        | <span data-ttu-id="43910-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43910-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="43910-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43910-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="43910-111">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="43910-111">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="43910-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43910-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43910-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43910-113">Not supported.</span></span>                              |
| <span data-ttu-id="43910-114">Application</span><span class="sxs-lookup"><span data-stu-id="43910-114">Application</span></span>                            | <span data-ttu-id="43910-115">InformationProtectionPolicy. Read. All</span><span class="sxs-lookup"><span data-stu-id="43910-115">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="43910-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43910-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationprotection/policy/labels/{id}
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43910-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="43910-117">Optional query parameters</span></span>

<span data-ttu-id="43910-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="43910-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="43910-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="43910-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="43910-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43910-120">Request headers</span></span>

| <span data-ttu-id="43910-121">Nome</span><span class="sxs-lookup"><span data-stu-id="43910-121">Name</span></span>          | <span data-ttu-id="43910-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="43910-122">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="43910-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="43910-123">Authorization</span></span> | <span data-ttu-id="43910-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43910-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="43910-126">Agente de usuário</span><span class="sxs-lookup"><span data-stu-id="43910-126">User-Agent</span></span>    | <span data-ttu-id="43910-127">Descreve o nome e a versão do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="43910-127">Describes the name and version of the calling application.</span></span> <span data-ttu-id="43910-128">Os detalhes surgirão no Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="43910-128">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="43910-129">O formato sugerido é ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="43910-129">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="43910-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="43910-130">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43910-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43910-131">Request body</span></span>

<span data-ttu-id="43910-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43910-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43910-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="43910-133">Response</span></span>

<span data-ttu-id="43910-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [informationProtectionLabel](../resources/informationprotectionlabel.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43910-134">If successful, this method returns a `200 OK` response code and the requested [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43910-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="43910-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43910-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43910-136">Request</span></span>

<span data-ttu-id="43910-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43910-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="43910-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="43910-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="43910-139">C#</span><span class="sxs-lookup"><span data-stu-id="43910-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-informationprotectionlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43910-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43910-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-informationprotectionlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="43910-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43910-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-informationprotectionlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="43910-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="43910-142">Response</span></span>

<span data-ttu-id="43910-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43910-143">The following is an example of the response.</span></span>

> <span data-ttu-id="43910-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43910-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionLabel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
User-agent: ContosoLOBApp/1.0

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('1e36d926-d716-4197-ba86-a6e18eb910b9')/informationProtection/policy/labels/$entity",
    "id": "4662f9a3-dd50-4a20-b984-a7be82e0e79c",
    "name": "LabelWithFooterAndHeaderActions_Tests",
    "description": "",
    "color": "",
    "sensitivity": 12,
    "tooltip": "LabelWithFooterAndHeaderActions_Tests",
    "isActive": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get informationProtectionLabel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
