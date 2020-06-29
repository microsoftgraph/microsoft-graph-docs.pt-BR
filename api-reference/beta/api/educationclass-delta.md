---
title: 'educationClass: Delta'
description: Obter classes recém-criadas ou atualizadas, incluindo as alterações de associação, sem ter que realizar uma leitura completa de toda a coleção de classes.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3b86b0c7fb39e274c553811ebb2a838613efedff
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909546"
---
# <a name="educationclass-delta"></a><span data-ttu-id="f81f6-103">educationClass: Delta</span><span class="sxs-lookup"><span data-stu-id="f81f6-103">educationClass: delta</span></span>

<span data-ttu-id="f81f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f81f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f81f6-105">Obter classes recém-criadas ou atualizadas, incluindo as alterações de associação, sem ter que realizar uma leitura completa de toda a coleção de classes.</span><span class="sxs-lookup"><span data-stu-id="f81f6-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="f81f6-106">Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="f81f6-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="f81f6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f81f6-107">Permissions</span></span>

<span data-ttu-id="f81f6-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f81f6-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f81f6-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f81f6-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f81f6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f81f6-110">Permission type</span></span>                        | <span data-ttu-id="f81f6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f81f6-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="f81f6-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f81f6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f81f6-113">EduRoster. ReadBasic, EduRoster. Read ou EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f81f6-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="f81f6-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f81f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f81f6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f81f6-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="f81f6-116">Application</span><span class="sxs-lookup"><span data-stu-id="f81f6-116">Application</span></span>                            | <span data-ttu-id="f81f6-117">EduRoster. ReadBasic. All, EduRoster. Read. All ou EduRoster. WriteWrite. All</span><span class="sxs-lookup"><span data-stu-id="f81f6-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f81f6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f81f6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/classes/{id}/delta
POST /education/me/classes/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="f81f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f81f6-119">Request headers</span></span>

| <span data-ttu-id="f81f6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f81f6-120">Name</span></span>          | <span data-ttu-id="f81f6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f81f6-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="f81f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f81f6-122">Authorization</span></span> | <span data-ttu-id="f81f6-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f81f6-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f81f6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f81f6-124">Request body</span></span>

<span data-ttu-id="f81f6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f81f6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f81f6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f81f6-126">Response</span></span>

<span data-ttu-id="f81f6-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f81f6-127">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f81f6-128">educationClass deltas não incluem classes excluídas.</span><span class="sxs-lookup"><span data-stu-id="f81f6-128">educationClass deltas do not include deleted classes.</span></span>

## <a name="example"></a><span data-ttu-id="f81f6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f81f6-129">Example</span></span>

<span data-ttu-id="f81f6-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f81f6-130">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f81f6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f81f6-131">Request</span></span>

<span data-ttu-id="f81f6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f81f6-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/{id}/delta
```

##### <a name="response"></a><span data-ttu-id="f81f6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f81f6-133">Response</span></span>

<span data-ttu-id="f81f6-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f81f6-134">The following is an example of the response.</span></span>

> <span data-ttu-id="f81f6-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="f81f6-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f81f6-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f81f6-136">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 585

{
  "value": [
    {
      "displayName": "displayName-value",
      "mailNickname": "mailNickname-value",
      "description": "description-value",
      "createdBy": {
        "application": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "device": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "user": {
          "displayName": "displayName-value",
          "id": "id-value"
        }
      },
      "classCode": "classCode-value",
      "externalName": "externalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
