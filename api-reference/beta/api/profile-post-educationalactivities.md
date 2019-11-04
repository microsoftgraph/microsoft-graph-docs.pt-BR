---
title: Criar educationalActivity
description: Criar um novo educationalActivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9d860955227de6b85f110c794e264559586fa172
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937711"
---
# <a name="create-educationalactivity"></a><span data-ttu-id="dcaca-103">Criar educationalActivity</span><span class="sxs-lookup"><span data-stu-id="dcaca-103">Create educationalActivity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcaca-104">Criar um novo [educationalActivity](../resources/educationalactivity.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="dcaca-104">Create a new [educationalActivity](../resources/educationalactivity.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcaca-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcaca-105">Permissions</span></span>

<span data-ttu-id="dcaca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcaca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcaca-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcaca-108">Permission type</span></span>                        | <span data-ttu-id="dcaca-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcaca-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dcaca-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcaca-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcaca-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dcaca-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="dcaca-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcaca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcaca-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dcaca-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="dcaca-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcaca-114">Application</span></span>                            | <span data-ttu-id="dcaca-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcaca-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcaca-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcaca-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/educationalActivities
```

## <a name="request-headers"></a><span data-ttu-id="dcaca-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcaca-117">Request headers</span></span>

| <span data-ttu-id="dcaca-118">Nome</span><span class="sxs-lookup"><span data-stu-id="dcaca-118">Name</span></span>      |<span data-ttu-id="dcaca-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcaca-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dcaca-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcaca-120">Authorization</span></span>  | <span data-ttu-id="dcaca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcaca-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="dcaca-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dcaca-123">Content-Type</span></span>   | <span data-ttu-id="dcaca-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcaca-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcaca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcaca-126">Request body</span></span>

<span data-ttu-id="dcaca-127">No corpo da solicitação, forneça uma representação JSON de um objeto [educationalActivity](../resources/educationalactivity.md) .</span><span class="sxs-lookup"><span data-stu-id="dcaca-127">In the request body, supply a JSON representation of an [educationalActivity](../resources/educationalactivity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dcaca-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcaca-128">Response</span></span>

<span data-ttu-id="dcaca-129">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [educationalActivity](../resources/educationalactivity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcaca-129">If successful, this method returns a `201 Created` response code and a new [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcaca-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dcaca-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dcaca-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcaca-131">Request</span></span>

<span data-ttu-id="dcaca-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcaca-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationalactivity_from_profile"
}-->

```http
POST /me/profile/educationalActivities
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

### <a name="response"></a><span data-ttu-id="dcaca-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcaca-133">Response</span></span>

<span data-ttu-id="dcaca-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcaca-134">The following is an example of the response.</span></span>

> <span data-ttu-id="dcaca-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcaca-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
