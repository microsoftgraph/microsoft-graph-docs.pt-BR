---
title: 'educationClass: Delta'
description: Obter classes recém-criadas ou atualizadas, incluindo as alterações de associação, sem ter que realizar uma leitura completa de toda a coleção de classes.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 03a026a479c9502e00b86e41936619613013b9af
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764723"
---
# <a name="educationclass-delta"></a><span data-ttu-id="5974f-103">educationClass: Delta</span><span class="sxs-lookup"><span data-stu-id="5974f-103">educationClass: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5974f-104">Obter classes recém-criadas ou atualizadas, incluindo as alterações de associação, sem ter que realizar uma leitura completa de toda a coleção de classes.</span><span class="sxs-lookup"><span data-stu-id="5974f-104">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="5974f-105">Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="5974f-105">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="5974f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5974f-106">Permissions</span></span>

<span data-ttu-id="5974f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5974f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5974f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5974f-109">Permission type</span></span>                        | <span data-ttu-id="5974f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5974f-110">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="5974f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5974f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5974f-112">EduRoster. ReadBasic, EduRoster. Read ou EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5974f-112">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="5974f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5974f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5974f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5974f-114">Not supported.</span></span>                                                           |
| <span data-ttu-id="5974f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5974f-115">Application</span></span>                            | <span data-ttu-id="5974f-116">EduRoster. ReadBasic. All, EduRoster. Read. All ou EduRoster. WriteWrite. All</span><span class="sxs-lookup"><span data-stu-id="5974f-116">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5974f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5974f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/classes/{id}/delta
POST /education/me/classes/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="5974f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5974f-118">Request headers</span></span>

| <span data-ttu-id="5974f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5974f-119">Name</span></span>          | <span data-ttu-id="5974f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5974f-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="5974f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5974f-121">Authorization</span></span> | <span data-ttu-id="5974f-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5974f-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5974f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5974f-123">Request body</span></span>

<span data-ttu-id="5974f-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5974f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5974f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="5974f-125">Response</span></span>

<span data-ttu-id="5974f-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5974f-126">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5974f-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5974f-127">Example</span></span>

<span data-ttu-id="5974f-128">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5974f-128">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5974f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5974f-129">Request</span></span>

<span data-ttu-id="5974f-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5974f-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/{id}/delta
```

##### <a name="response"></a><span data-ttu-id="5974f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5974f-131">Response</span></span>

<span data-ttu-id="5974f-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5974f-132">The following is an example of the response.</span></span> 

><span data-ttu-id="5974f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5974f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
