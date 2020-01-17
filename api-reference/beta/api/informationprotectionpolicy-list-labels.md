---
title: 'informationProtectionLabel: listLabels'
description: Recupere uma lista de rótulos de proteção de informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c3e83fd6d7fa19da70010136c3bec85ce17b694a
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216254"
---
# <a name="informationprotectionlabel-listlabels"></a><span data-ttu-id="a3e0e-103">informationProtectionLabel: listLabels</span><span class="sxs-lookup"><span data-stu-id="a3e0e-103">informationProtectionLabel: listLabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3e0e-104">Obtenha um conjunto de [Rótulos de proteção de informações](../resources/informationprotectionlabel.md) disponíveis para o usuário ou para a organização.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-104">Get a collection of [information protection labels](../resources/informationprotectionlabel.md) available to the user or to the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3e0e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3e0e-105">Permissions</span></span>

<span data-ttu-id="a3e0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3e0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3e0e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3e0e-108">Permission type</span></span>                        | <span data-ttu-id="a3e0e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3e0e-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a3e0e-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3e0e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3e0e-111">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="a3e0e-111">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="a3e0e-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3e0e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3e0e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-113">Not supported.</span></span>                              |
| <span data-ttu-id="a3e0e-114">Application</span><span class="sxs-lookup"><span data-stu-id="a3e0e-114">Application</span></span>                            | <span data-ttu-id="a3e0e-115">InformationProtectionPolicy. Read. All</span><span class="sxs-lookup"><span data-stu-id="a3e0e-115">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="a3e0e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3e0e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/informationprotection/policy/labels
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3e0e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a3e0e-117">Optional query parameters</span></span>

<span data-ttu-id="a3e0e-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a3e0e-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a3e0e-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3e0e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3e0e-120">Request headers</span></span>

| <span data-ttu-id="a3e0e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a3e0e-121">Name</span></span>          | <span data-ttu-id="a3e0e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3e0e-122">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a3e0e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3e0e-123">Authorization</span></span> | <span data-ttu-id="a3e0e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="a3e0e-126">Agente de usuário</span><span class="sxs-lookup"><span data-stu-id="a3e0e-126">User-Agent</span></span>    | <span data-ttu-id="a3e0e-127">Descreve o nome e a versão do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-127">Describes the name and version of the calling application.</span></span> <span data-ttu-id="a3e0e-128">Os detalhes surgirão no Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-128">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="a3e0e-129">O formato sugerido é ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-129">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="a3e0e-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-130">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3e0e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3e0e-131">Request body</span></span>

<span data-ttu-id="a3e0e-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3e0e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3e0e-133">Response</span></span>

<span data-ttu-id="a3e0e-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [informationProtectionLabel](../resources/informationprotectionlabel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-134">If successful, this method returns a `200 OK` response code and a collection of [informationProtectionLabel](../resources/informationprotectionlabel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3e0e-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a3e0e-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3e0e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3e0e-136">Request</span></span>

<span data-ttu-id="a3e0e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a3e0e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3e0e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_labels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a3e0e-139">C#</span><span class="sxs-lookup"><span data-stu-id="a3e0e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-labels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3e0e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3e0e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-labels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a3e0e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3e0e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-labels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a3e0e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3e0e-142">Response</span></span>

<span data-ttu-id="a3e0e-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-143">The following is an example of the response.</span></span>

> <span data-ttu-id="a3e0e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3e0e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
User-agent: ContosoLOBApp/1.0

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('1e36d926-d716-4197-ba86-a6e18eb910b9')/informationProtection/policy/labels",
  "value": [
      {
          "id": "3a80e051-487c-40d4-b491-73ad25d997e6",
          "name": "General",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 1,
          "tooltip": "Data classified as Contoso General.",
          "isActive": true
      },
      {
          "id": "4662f9a3-dd50-4a20-b984-a7be82e0e79c",
          "name": "Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 2,
          "tooltip": "Data classificed as Contoso Confidential.",
          "isActive": true
      },
      {
          "id": "4b18e8bb-b4a5-4695-85d0-8ae23ef27892",
          "name": "Highly Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 3,
          "tooltip": "Data classified as Contoso Highly Confidential.",
          "isActive": true
      }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List labels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
