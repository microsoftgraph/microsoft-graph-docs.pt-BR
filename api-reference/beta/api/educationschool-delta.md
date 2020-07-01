---
title: 'educationSchool: Delta'
description: Obter escolas recém-criadas ou atualizadas sem ter que realizar uma leitura completa de toda a coleção de escola.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 160c7cf9e897f485e9c4e33c3fe579e78e277e79
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006839"
---
# <a name="educationschool-delta"></a><span data-ttu-id="43228-103">educationSchool: Delta</span><span class="sxs-lookup"><span data-stu-id="43228-103">educationSchool: delta</span></span>

<span data-ttu-id="43228-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43228-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43228-105">Obter escolas recém-criadas ou atualizadas sem ter que realizar uma leitura completa de toda a coleção de escola.</span><span class="sxs-lookup"><span data-stu-id="43228-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span></span> <span data-ttu-id="43228-106">Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="43228-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="43228-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="43228-107">Permissions</span></span>

<span data-ttu-id="43228-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="43228-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="43228-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43228-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43228-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43228-110">Permission type</span></span>                        | <span data-ttu-id="43228-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43228-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="43228-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43228-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="43228-113">EduRoster. ReadBasic, EduRoster. Read ou EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43228-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="43228-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43228-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43228-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43228-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="43228-116">Application</span><span class="sxs-lookup"><span data-stu-id="43228-116">Application</span></span>                            | <span data-ttu-id="43228-117">EduRoster. ReadBasic. All, EduRoster. Read. All ou EduRoster. WriteWrite. All</span><span class="sxs-lookup"><span data-stu-id="43228-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43228-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43228-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/schools/delta
```

## <a name="request-headers"></a><span data-ttu-id="43228-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43228-119">Request headers</span></span>

| <span data-ttu-id="43228-120">Nome</span><span class="sxs-lookup"><span data-stu-id="43228-120">Name</span></span>          | <span data-ttu-id="43228-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="43228-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="43228-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="43228-122">Authorization</span></span> | <span data-ttu-id="43228-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="43228-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="43228-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43228-124">Request body</span></span>

<span data-ttu-id="43228-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43228-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43228-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="43228-126">Response</span></span>

<span data-ttu-id="43228-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43228-127">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="43228-128">educationSchool deltas não incluem escolas excluídas.</span><span class="sxs-lookup"><span data-stu-id="43228-128">educationSchool deltas do not include deleted schools.</span></span>

## <a name="example"></a><span data-ttu-id="43228-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43228-129">Example</span></span>

<span data-ttu-id="43228-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="43228-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="43228-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43228-131">Request</span></span>

<span data-ttu-id="43228-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43228-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```http
GET https://graph.microsoft.com/beta/education/schools/delta
```

### <a name="response"></a><span data-ttu-id="43228-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="43228-133">Response</span></span>

<span data-ttu-id="43228-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43228-134">The following is an example of the response.</span></span>

> <span data-ttu-id="43228-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="43228-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="43228-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="43228-136">All the properties will be returned from an actual call.</span></span>

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
