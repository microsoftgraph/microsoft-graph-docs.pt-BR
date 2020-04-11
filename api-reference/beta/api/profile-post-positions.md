---
title: Criar workPosition
description: Use esta API para criar um novo workPosition.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0344dc0d0f861fb653f1ed26e2b951978148c8b8
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229308"
---
# <a name="create-workposition"></a><span data-ttu-id="034c4-103">Criar workPosition</span><span class="sxs-lookup"><span data-stu-id="034c4-103">Create workPosition</span></span>

<span data-ttu-id="034c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="034c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="034c4-105">Use esta API para criar um novo [workPosition](../resources/workposition.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="034c4-105">Use this API to create a new [workPosition](../resources/workposition.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="034c4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="034c4-106">Permissions</span></span>

<span data-ttu-id="034c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="034c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="034c4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="034c4-109">Permission type</span></span>                        | <span data-ttu-id="034c4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="034c4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="034c4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="034c4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="034c4-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="034c4-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="034c4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="034c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="034c4-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="034c4-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="034c4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="034c4-115">Application</span></span>                            | <span data-ttu-id="034c4-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="034c4-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="034c4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="034c4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/positions
```

## <a name="request-headers"></a><span data-ttu-id="034c4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="034c4-118">Request headers</span></span>

| <span data-ttu-id="034c4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="034c4-119">Name</span></span>      |<span data-ttu-id="034c4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="034c4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="034c4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="034c4-121">Authorization</span></span>  | <span data-ttu-id="034c4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="034c4-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="034c4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="034c4-124">Content-Type</span></span>   | <span data-ttu-id="034c4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="034c4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="034c4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="034c4-127">Request body</span></span>

<span data-ttu-id="034c4-128">No corpo da solicitação, forneça uma representação JSON do objeto [workPosition](../resources/workposition.md) .</span><span class="sxs-lookup"><span data-stu-id="034c4-128">In the request body, supply a JSON representation of [workPosition](../resources/workposition.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="034c4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="034c4-129">Response</span></span>

<span data-ttu-id="034c4-130">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [workPosition](../resources/workposition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="034c4-130">If successful, this method returns `201, Created` response code and a new [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="034c4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="034c4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="034c4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="034c4-132">Request</span></span>

<span data-ttu-id="034c4-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="034c4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_workposition_from_profile"
}-->

```http
POST https://graph.microsoft.com/Beta/me/profile/positions
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
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
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  }
}
```

### <a name="response"></a><span data-ttu-id="034c4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="034c4-134">Response</span></span>

<span data-ttu-id="034c4-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="034c4-135">The following is an example of the response.</span></span>

> <span data-ttu-id="034c4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="034c4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
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
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->