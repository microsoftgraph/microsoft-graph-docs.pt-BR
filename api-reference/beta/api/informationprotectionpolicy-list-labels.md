---
title: 'informationProtectionLabel: listLabels'
description: Recupere uma lista de rótulos de proteção de informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 94b47a2bac3e3000af5123bf2a7b4dd88c43e0cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446335"
---
# <a name="informationprotectionlabel-listlabels"></a><span data-ttu-id="a1551-103">informationProtectionLabel: listLabels</span><span class="sxs-lookup"><span data-stu-id="a1551-103">informationProtectionLabel: listLabels</span></span>

<span data-ttu-id="a1551-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a1551-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1551-105">Obtenha um conjunto de [Rótulos de proteção de informações](../resources/informationprotectionlabel.md) disponíveis para o usuário ou para a organização.</span><span class="sxs-lookup"><span data-stu-id="a1551-105">Get a collection of [information protection labels](../resources/informationprotectionlabel.md) available to the user or to the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1551-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1551-106">Permissions</span></span>

<span data-ttu-id="a1551-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1551-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1551-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1551-109">Permission type</span></span>                        | <span data-ttu-id="a1551-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1551-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a1551-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1551-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1551-112">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="a1551-112">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="a1551-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1551-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1551-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1551-114">Not supported.</span></span>                              |
| <span data-ttu-id="a1551-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1551-115">Application</span></span>                            | <span data-ttu-id="a1551-116">InformationProtectionPolicy. Read. All</span><span class="sxs-lookup"><span data-stu-id="a1551-116">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="a1551-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1551-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/informationprotection/policy/labels
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1551-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1551-118">Optional query parameters</span></span>

<span data-ttu-id="a1551-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1551-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a1551-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a1551-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1551-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1551-121">Request headers</span></span>

| <span data-ttu-id="a1551-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a1551-122">Name</span></span>          | <span data-ttu-id="a1551-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1551-123">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a1551-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1551-124">Authorization</span></span> | <span data-ttu-id="a1551-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1551-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="a1551-127">Agente de usuário</span><span class="sxs-lookup"><span data-stu-id="a1551-127">User-Agent</span></span>    | <span data-ttu-id="a1551-128">Descreve o nome e a versão do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="a1551-128">Describes the name and version of the calling application.</span></span> <span data-ttu-id="a1551-129">Os detalhes surgirão no Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="a1551-129">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="a1551-130">O formato sugerido é ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="a1551-130">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="a1551-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a1551-131">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1551-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1551-132">Request body</span></span>

<span data-ttu-id="a1551-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1551-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1551-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1551-134">Response</span></span>

<span data-ttu-id="a1551-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [informationProtectionLabel](../resources/informationprotectionlabel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1551-135">If successful, this method returns a `200 OK` response code and a collection of [informationProtectionLabel](../resources/informationprotectionlabel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1551-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a1551-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1551-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1551-137">Request</span></span>

<span data-ttu-id="a1551-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1551-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1551-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1551-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_labels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels
```
# <a name="c"></a>[<span data-ttu-id="a1551-140">C#</span><span class="sxs-lookup"><span data-stu-id="a1551-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-labels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1551-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1551-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-labels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1551-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1551-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-labels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1551-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1551-143">Response</span></span>

<span data-ttu-id="a1551-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1551-144">The following is an example of the response.</span></span>

> <span data-ttu-id="a1551-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1551-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
