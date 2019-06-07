---
title: 'educationUser: Delta'
description: Obter usuários recém-criados ou atualizados sem ter que realizar uma leitura completa de toda a coleção de usuários.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c89c065d5e4bd8510d6821a3c7a13bd106ce9eb8
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764724"
---
# <a name="educationuser-delta"></a><span data-ttu-id="5a611-103">educationUser: Delta</span><span class="sxs-lookup"><span data-stu-id="5a611-103">educationUser: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a611-104">Obter [educationUser](../resources/educationuser.md) recentemente criados ou atualizados sem ter que realizar uma leitura completa de toda a coleção.</span><span class="sxs-lookup"><span data-stu-id="5a611-104">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="5a611-105">Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="5a611-105">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a611-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a611-106">Permissions</span></span>

<span data-ttu-id="5a611-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a611-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a611-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a611-109">Permission type</span></span>                        | <span data-ttu-id="5a611-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a611-110">Permissions (from least to most privileged)</span></span>     |
| :------------------------------------- | :---------------------------------------------- |
| <span data-ttu-id="5a611-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a611-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a611-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a611-112">Not supported.</span></span>                                  |
| <span data-ttu-id="5a611-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a611-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a611-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a611-114">Not supported.</span></span>                                  |
| <span data-ttu-id="5a611-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a611-115">Application</span></span>                            | <span data-ttu-id="5a611-116">EduRoster. Read. All ou EduRoster. WriteWrite. All</span><span class="sxs-lookup"><span data-stu-id="5a611-116">EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a611-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a611-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/delta
POST /education/users/{id}/delta
POST /education/schools/{id}/users/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="5a611-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a611-118">Request headers</span></span>

| <span data-ttu-id="5a611-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5a611-119">Name</span></span>          | <span data-ttu-id="5a611-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a611-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="5a611-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a611-121">Authorization</span></span> | <span data-ttu-id="5a611-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5a611-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a611-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a611-123">Request body</span></span>

<span data-ttu-id="5a611-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a611-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a611-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a611-125">Response</span></span>

<span data-ttu-id="5a611-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a611-126">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a611-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a611-127">Example</span></span>

<span data-ttu-id="5a611-128">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5a611-128">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5a611-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a611-129">Request</span></span>

<span data-ttu-id="5a611-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a611-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/me/delta
```

##### <a name="response"></a><span data-ttu-id="5a611-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a611-131">Response</span></span>

<span data-ttu-id="5a611-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5a611-132">The following is an example of the response.</span></span>

><span data-ttu-id="5a611-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a611-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
