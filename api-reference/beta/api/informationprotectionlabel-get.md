---
title: Obter informationProtectionLabel
description: Recupere as propriedades e as relações do objeto informationProtectionLabel especificado.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 8400ceb42bb9f35a00c844369f904ae791b08534
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954655"
---
# <a name="get-informationprotectionlabel"></a><span data-ttu-id="0a999-103">Obter informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="0a999-103">Get informationProtectionLabel</span></span>

<span data-ttu-id="0a999-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a999-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a999-105">Recupere as propriedades e as relações de um [objeto informationProtectionLabel.](../resources/informationprotectionlabel.md)</span><span class="sxs-lookup"><span data-stu-id="0a999-105">Retrieve the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a999-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a999-106">Permissions</span></span>

<span data-ttu-id="0a999-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a999-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a999-109">Permission type</span></span>                        | <span data-ttu-id="0a999-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a999-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="0a999-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a999-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a999-112">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="0a999-112">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="0a999-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a999-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a999-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a999-114">Not supported.</span></span>                              |
| <span data-ttu-id="0a999-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a999-115">Application</span></span>                            | <span data-ttu-id="0a999-116">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a999-116">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="0a999-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a999-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0a999-118">Para obter um rótulo disponível para o usuário ou usuário especificado:</span><span class="sxs-lookup"><span data-stu-id="0a999-118">To get a label available to the signed-in user or specified user:</span></span>
```http
GET /me/informationProtection/policy/labels/{id}
GET /users/{id | user-principal-name}/informationProtection/policy/labels/{id}
```

<span data-ttu-id="0a999-119">Para obter um rótulo disponível para a organização:</span><span class="sxs-lookup"><span data-stu-id="0a999-119">To get a label available to the organization:</span></span>
```http
GET /informationProtection/policy/labels/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a999-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0a999-120">Optional query parameters</span></span>

<span data-ttu-id="0a999-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0a999-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0a999-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0a999-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a999-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a999-123">Request headers</span></span>

| <span data-ttu-id="0a999-124">Nome</span><span class="sxs-lookup"><span data-stu-id="0a999-124">Name</span></span>          | <span data-ttu-id="0a999-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a999-125">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0a999-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a999-126">Authorization</span></span> | <span data-ttu-id="0a999-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a999-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="0a999-129">User-Agent</span><span class="sxs-lookup"><span data-stu-id="0a999-129">User-Agent</span></span>    | <span data-ttu-id="0a999-130">Descreve o nome e a versão do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="0a999-130">Describes the name and version of the calling application.</span></span> <span data-ttu-id="0a999-131">Os detalhes aparecerão no Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="0a999-131">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="0a999-132">O formato sugerido é ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="0a999-132">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="0a999-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0a999-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a999-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a999-134">Request body</span></span>

<span data-ttu-id="0a999-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0a999-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a999-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a999-136">Response</span></span>

<span data-ttu-id="0a999-137">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [informationProtectionLabel](../resources/informationprotectionlabel.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a999-137">If successful, this method returns a `200 OK` response code and the requested [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a999-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0a999-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a999-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a999-139">Request</span></span>

<span data-ttu-id="0a999-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a999-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a999-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a999-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels/{id}
```
# <a name="c"></a>[<span data-ttu-id="0a999-142">C#</span><span class="sxs-lookup"><span data-stu-id="0a999-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-informationprotectionlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a999-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a999-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-informationprotectionlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a999-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a999-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-informationprotectionlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a999-145">Java</span><span class="sxs-lookup"><span data-stu-id="0a999-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-informationprotectionlabel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a999-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a999-146">Response</span></span>

<span data-ttu-id="0a999-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0a999-147">The following is an example of the response.</span></span>

> <span data-ttu-id="0a999-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a999-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


