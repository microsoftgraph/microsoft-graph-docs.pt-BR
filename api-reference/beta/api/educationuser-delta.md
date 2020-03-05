---
title: 'educationUser: Delta'
description: Obter usuários recém-criados ou atualizados sem ter que realizar uma leitura completa de toda a coleção de usuários.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 37dc85ae1c907aaa1cf43428e7ad19188e7c053d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423921"
---
# <a name="educationuser-delta"></a><span data-ttu-id="58e4b-103">educationUser: Delta</span><span class="sxs-lookup"><span data-stu-id="58e4b-103">educationUser: delta</span></span>

<span data-ttu-id="58e4b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="58e4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58e4b-105">Obter [educationUser](../resources/educationuser.md) recentemente criados ou atualizados sem ter que realizar uma leitura completa de toda a coleção.</span><span class="sxs-lookup"><span data-stu-id="58e4b-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="58e4b-106">Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="58e4b-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="58e4b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="58e4b-107">Permissions</span></span>

<span data-ttu-id="58e4b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58e4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58e4b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58e4b-110">Permission type</span></span>                        | <span data-ttu-id="58e4b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58e4b-111">Permissions (from least to most privileged)</span></span>     |
| :------------------------------------- | :---------------------------------------------- |
| <span data-ttu-id="58e4b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58e4b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="58e4b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58e4b-113">Not supported.</span></span>                                  |
| <span data-ttu-id="58e4b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58e4b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58e4b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58e4b-115">Not supported.</span></span>                                  |
| <span data-ttu-id="58e4b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58e4b-116">Application</span></span>                            | <span data-ttu-id="58e4b-117">EduRoster. Read. All ou EduRoster. WriteWrite. All</span><span class="sxs-lookup"><span data-stu-id="58e4b-117">EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58e4b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58e4b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/delta
POST /education/users/{id}/delta
POST /education/schools/{id}/users/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="58e4b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58e4b-119">Request headers</span></span>

| <span data-ttu-id="58e4b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="58e4b-120">Name</span></span>          | <span data-ttu-id="58e4b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="58e4b-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="58e4b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58e4b-122">Authorization</span></span> | <span data-ttu-id="58e4b-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="58e4b-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="58e4b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58e4b-124">Request body</span></span>

<span data-ttu-id="58e4b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58e4b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58e4b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="58e4b-126">Response</span></span>

<span data-ttu-id="58e4b-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58e4b-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58e4b-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58e4b-128">Example</span></span>

<span data-ttu-id="58e4b-129">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="58e4b-129">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="58e4b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58e4b-130">Request</span></span>

<span data-ttu-id="58e4b-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="58e4b-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/me/delta
```

##### <a name="response"></a><span data-ttu-id="58e4b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="58e4b-132">Response</span></span>

<span data-ttu-id="58e4b-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="58e4b-133">The following is an example of the response.</span></span>

><span data-ttu-id="58e4b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58e4b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
