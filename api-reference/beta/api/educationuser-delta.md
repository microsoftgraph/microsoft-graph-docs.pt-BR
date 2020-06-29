---
title: 'educationUser: Delta'
description: Obter usuários recém-criados ou atualizados sem ter que realizar uma leitura completa de toda a coleção de usuários.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 408fb43dbad69cbb699db899522cf938e84ec904
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909545"
---
# <a name="educationuser-delta"></a><span data-ttu-id="94d9d-103">educationUser: Delta</span><span class="sxs-lookup"><span data-stu-id="94d9d-103">educationUser: delta</span></span>

<span data-ttu-id="94d9d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94d9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94d9d-105">Obter [educationUser](../resources/educationuser.md) recentemente criados ou atualizados sem ter que realizar uma leitura completa de toda a coleção.</span><span class="sxs-lookup"><span data-stu-id="94d9d-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="94d9d-106">Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="94d9d-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="94d9d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="94d9d-107">Permissions</span></span>

<span data-ttu-id="94d9d-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="94d9d-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="94d9d-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94d9d-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94d9d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94d9d-110">Permission type</span></span>                        | <span data-ttu-id="94d9d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94d9d-111">Permissions (from least to most privileged)</span></span>     |
| :------------------------------------- | :---------------------------------------------- |
| <span data-ttu-id="94d9d-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94d9d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="94d9d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94d9d-113">Not supported.</span></span>                                  |
| <span data-ttu-id="94d9d-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94d9d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94d9d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94d9d-115">Not supported.</span></span>                                  |
| <span data-ttu-id="94d9d-116">Application</span><span class="sxs-lookup"><span data-stu-id="94d9d-116">Application</span></span>                            | <span data-ttu-id="94d9d-117">EduRoster. Read. All ou EduRoster. WriteWrite. All</span><span class="sxs-lookup"><span data-stu-id="94d9d-117">EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94d9d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94d9d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/delta
POST /education/users/{id}/delta
POST /education/schools/{id}/users/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="94d9d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94d9d-119">Request headers</span></span>

| <span data-ttu-id="94d9d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="94d9d-120">Name</span></span>          | <span data-ttu-id="94d9d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="94d9d-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="94d9d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94d9d-122">Authorization</span></span> | <span data-ttu-id="94d9d-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="94d9d-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="94d9d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94d9d-124">Request body</span></span>

<span data-ttu-id="94d9d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94d9d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94d9d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="94d9d-126">Response</span></span>

<span data-ttu-id="94d9d-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94d9d-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="94d9d-128">educationUser deltas não incluem usuários excluídos.</span><span class="sxs-lookup"><span data-stu-id="94d9d-128">educationUser deltas do not include deleted users.</span></span>

## <a name="example"></a><span data-ttu-id="94d9d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94d9d-129">Example</span></span>

<span data-ttu-id="94d9d-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="94d9d-130">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="94d9d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94d9d-131">Request</span></span>

<span data-ttu-id="94d9d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94d9d-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/me/delta
```

##### <a name="response"></a><span data-ttu-id="94d9d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="94d9d-133">Response</span></span>

<span data-ttu-id="94d9d-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94d9d-134">The following is an example of the response.</span></span>

> <span data-ttu-id="94d9d-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="94d9d-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="94d9d-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="94d9d-136">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1039

{
  "value": [
    {
      "primaryRole": "primaryRole-value",
      "middleName": "middleName-value",
      "externalSource": "externalSource-value",
      "residenceAddress": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "mailingAddress": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "student": {
        "graduationYear": "graduationYear-value",
        "grade": "grade-value",
        "birthDate": "datetime-value",
        "gender": "gender-value",
        "studentNumber": "studentNumber-value",
        "externalId": "externalId-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
