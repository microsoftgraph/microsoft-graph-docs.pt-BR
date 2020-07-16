---
title: 'educationSchool: Delta'
description: Obter escolas recém-criadas ou atualizadas sem ter que realizar uma leitura completa de toda a coleção de escola.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 43ee6465aae4ec668fda95775a846b2c51aa13b2
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081165"
---
# <a name="educationschool-delta"></a><span data-ttu-id="5fb2f-103">educationSchool: Delta</span><span class="sxs-lookup"><span data-stu-id="5fb2f-103">educationSchool: delta</span></span>

<span data-ttu-id="5fb2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fb2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fb2f-105">Obter escolas recém-criadas ou atualizadas sem ter que realizar uma leitura completa de toda a coleção de escola.</span><span class="sxs-lookup"><span data-stu-id="5fb2f-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span></span> <span data-ttu-id="5fb2f-106">Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="5fb2f-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fb2f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5fb2f-107">Permissions</span></span>

<span data-ttu-id="5fb2f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fb2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5fb2f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fb2f-110">Permission type</span></span>                        | <span data-ttu-id="5fb2f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5fb2f-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="5fb2f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fb2f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5fb2f-113">EduRoster. ReadBasic, EduRoster. Read ou EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5fb2f-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="5fb2f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fb2f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fb2f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fb2f-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="5fb2f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fb2f-116">Application</span></span>                            | <span data-ttu-id="5fb2f-117">EduRoster. ReadBasic. All, EduRoster. Read. All ou EduRoster. WriteWrite. All</span><span class="sxs-lookup"><span data-stu-id="5fb2f-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fb2f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fb2f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/schools/delta
```

## <a name="request-headers"></a><span data-ttu-id="5fb2f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fb2f-119">Request headers</span></span>

| <span data-ttu-id="5fb2f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5fb2f-120">Name</span></span>          | <span data-ttu-id="5fb2f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fb2f-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="5fb2f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fb2f-122">Authorization</span></span> | <span data-ttu-id="5fb2f-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5fb2f-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5fb2f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fb2f-124">Request body</span></span>

<span data-ttu-id="5fb2f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5fb2f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fb2f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fb2f-126">Response</span></span>

<span data-ttu-id="5fb2f-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fb2f-127">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5fb2f-128">educationSchool deltas não incluem escolas excluídas.</span><span class="sxs-lookup"><span data-stu-id="5fb2f-128">educationSchool deltas do not include deleted schools.</span></span>

## <a name="example"></a><span data-ttu-id="5fb2f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5fb2f-129">Example</span></span>

<span data-ttu-id="5fb2f-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5fb2f-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5fb2f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fb2f-131">Request</span></span>

<span data-ttu-id="5fb2f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fb2f-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5fb2f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fb2f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/delta
```
# <a name="c"></a>[<span data-ttu-id="5fb2f-134">C#</span><span class="sxs-lookup"><span data-stu-id="5fb2f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fb2f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fb2f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fb2f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fb2f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5fb2f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fb2f-137">Response</span></span>

<span data-ttu-id="5fb2f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5fb2f-138">The following is an example of the response.</span></span>

> <span data-ttu-id="5fb2f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5fb2f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "address": { "@odata.type": "microsoft.graph.physicalAddress" },
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "description": "String",
      "displayName": "String",
      "externalId": "String",
      "externalPrincipalId": "String",
      "externalSource": "string",
      "highestGrade": "String",
      "id": "String (identifier)",
      "lowestGrade": "String",
      "phone": "String",
      "principalEmail": "String",
      "principalName": "String",
      "schoolNumber": "String"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
