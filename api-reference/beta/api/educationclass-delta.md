---
title: 'educationClass: Delta'
description: Obter classes recém-criadas ou atualizadas, incluindo as alterações de associação, sem ter que realizar uma leitura completa de toda a coleção de classes.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 874898b68bcdb1d4bfc450668ebff89030859a02
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426875"
---
# <a name="educationclass-delta"></a><span data-ttu-id="29ac5-103">educationClass: Delta</span><span class="sxs-lookup"><span data-stu-id="29ac5-103">educationClass: delta</span></span>

<span data-ttu-id="29ac5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="29ac5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29ac5-105">Obter classes recém-criadas ou atualizadas, incluindo as alterações de associação, sem ter que realizar uma leitura completa de toda a coleção de classes.</span><span class="sxs-lookup"><span data-stu-id="29ac5-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="29ac5-106">Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="29ac5-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="29ac5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="29ac5-107">Permissions</span></span>

<span data-ttu-id="29ac5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29ac5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29ac5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29ac5-110">Permission type</span></span>                        | <span data-ttu-id="29ac5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29ac5-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="29ac5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29ac5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="29ac5-113">EduRoster. ReadBasic, EduRoster. Read ou EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29ac5-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="29ac5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29ac5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29ac5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29ac5-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="29ac5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29ac5-116">Application</span></span>                            | <span data-ttu-id="29ac5-117">EduRoster. ReadBasic. All, EduRoster. Read. All ou EduRoster. WriteWrite. All</span><span class="sxs-lookup"><span data-stu-id="29ac5-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29ac5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29ac5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/classes/{id}/delta
POST /education/me/classes/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="29ac5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29ac5-119">Request headers</span></span>

| <span data-ttu-id="29ac5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="29ac5-120">Name</span></span>          | <span data-ttu-id="29ac5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="29ac5-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="29ac5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="29ac5-122">Authorization</span></span> | <span data-ttu-id="29ac5-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="29ac5-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="29ac5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29ac5-124">Request body</span></span>

<span data-ttu-id="29ac5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29ac5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29ac5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="29ac5-126">Response</span></span>

<span data-ttu-id="29ac5-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29ac5-127">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29ac5-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29ac5-128">Example</span></span>

<span data-ttu-id="29ac5-129">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="29ac5-129">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="29ac5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29ac5-130">Request</span></span>

<span data-ttu-id="29ac5-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29ac5-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/{id}/delta
```

##### <a name="response"></a><span data-ttu-id="29ac5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="29ac5-132">Response</span></span>

<span data-ttu-id="29ac5-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29ac5-133">The following is an example of the response.</span></span> 

><span data-ttu-id="29ac5-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29ac5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
