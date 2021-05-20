---
title: 'informationProtectionLabel: listLabels'
description: Recupere uma lista de rótulos de proteção de informações.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 1be094a546bb34bc72bfc95e651bb502c0000f75
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579603"
---
# <a name="informationprotectionlabel-listlabels"></a><span data-ttu-id="682fa-103">informationProtectionLabel: listLabels</span><span class="sxs-lookup"><span data-stu-id="682fa-103">informationProtectionLabel: listLabels</span></span>

<span data-ttu-id="682fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="682fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="682fa-105">Obter uma coleção de [rótulos](../resources/informationprotectionlabel.md) de proteção de informações disponíveis para o usuário ou para a organização.</span><span class="sxs-lookup"><span data-stu-id="682fa-105">Get a collection of [information protection labels](../resources/informationprotectionlabel.md) available to the user or to the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="682fa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="682fa-106">Permissions</span></span>

<span data-ttu-id="682fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="682fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="682fa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="682fa-109">Permission type</span></span>                        | <span data-ttu-id="682fa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="682fa-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="682fa-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="682fa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="682fa-112">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="682fa-112">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="682fa-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="682fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="682fa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="682fa-114">Not supported.</span></span>                              |
| <span data-ttu-id="682fa-115">Application</span><span class="sxs-lookup"><span data-stu-id="682fa-115">Application</span></span>                            | <span data-ttu-id="682fa-116">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="682fa-116">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="682fa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="682fa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
<span data-ttu-id="682fa-118">Para obter rótulos disponíveis para o usuário ou usuário especificado:</span><span class="sxs-lookup"><span data-stu-id="682fa-118">To get labels available to the signed-in user or specified user:</span></span>
```http
GET /me/informationProtection/policy/labels
GET /users/{id | user-principal-name}/informationProtection/policy/labels
```

<span data-ttu-id="682fa-119">Para obter rótulos disponíveis para a organização:</span><span class="sxs-lookup"><span data-stu-id="682fa-119">To get labels available to the organization:</span></span>
```http
GET /informationProtection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="682fa-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="682fa-120">Optional query parameters</span></span>

<span data-ttu-id="682fa-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="682fa-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="682fa-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="682fa-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="682fa-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="682fa-123">Request headers</span></span>

| <span data-ttu-id="682fa-124">Nome</span><span class="sxs-lookup"><span data-stu-id="682fa-124">Name</span></span>          | <span data-ttu-id="682fa-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="682fa-125">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="682fa-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="682fa-126">Authorization</span></span> | <span data-ttu-id="682fa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="682fa-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="682fa-129">User-Agent</span><span class="sxs-lookup"><span data-stu-id="682fa-129">User-Agent</span></span>    | <span data-ttu-id="682fa-130">Descreve o nome e a versão do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="682fa-130">Describes the name and version of the calling application.</span></span> <span data-ttu-id="682fa-131">Os detalhes aparecerão no Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="682fa-131">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="682fa-132">O formato sugerido é ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="682fa-132">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="682fa-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="682fa-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="682fa-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="682fa-134">Request body</span></span>

<span data-ttu-id="682fa-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="682fa-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="682fa-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="682fa-136">Response</span></span>

<span data-ttu-id="682fa-137">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos informationProtectionLabel](../resources/informationprotectionlabel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="682fa-137">If successful, this method returns a `200 OK` response code and a collection of [informationProtectionLabel](../resources/informationprotectionlabel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="682fa-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="682fa-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="682fa-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="682fa-139">Request</span></span>

<span data-ttu-id="682fa-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="682fa-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="682fa-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="682fa-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_labels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationProtection/policy/labels
```
# <a name="c"></a>[<span data-ttu-id="682fa-142">C#</span><span class="sxs-lookup"><span data-stu-id="682fa-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-labels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="682fa-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="682fa-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-labels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="682fa-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="682fa-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-labels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="682fa-145">Java</span><span class="sxs-lookup"><span data-stu-id="682fa-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-labels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="682fa-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="682fa-146">Response</span></span>

<span data-ttu-id="682fa-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="682fa-147">The following is an example of the response.</span></span>

> <span data-ttu-id="682fa-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="682fa-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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
          "isActive": true,
          "parent": null
      },
      {
          "id": "4662f9a3-dd50-4a20-b984-a7be82e0e79c",
          "name": "Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 2,
          "tooltip": "Data classificed as Contoso Confidential.",
          "isActive": true,
          "parent": null
      },
      {
          "id": "4b18e8bb-b4a5-4695-85d0-8ae23ef27892",
          "name": "Highly Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 3,
          "tooltip": "Data classified as Contoso Highly Confidential.",
          "isActive": true,
          "parent": null
      },
      {
            "id": "a20cbae4-0c05-448c-b342-cb6c618d0957",
            "name": "Contoso Full Time Employees",
            "description": "Consult Contoso data labeling policy for more details.",
            "color": "",
            "sensitivity": 4,
            "tooltip": "Data classified as Contoso Highly Confidential for Contoso Full Time Employees",
            "isActive": true,
            "parent": {
                "id": "4b18e8bb-b4a5-4695-85d0-8ae23ef27892",
                "name": "Highly Confidential",
                "description": "Consult Contoso data labeling policy for more details.",
                "color": "",
                "sensitivity": 3,
                "tooltip": "Data classified as Contoso Highly Confidential.",
                "isActive": true,
                "parent": null
            }
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


