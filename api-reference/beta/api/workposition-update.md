---
title: Atualizar workPosition
description: Atualiza as propriedades de um objeto workPosition no perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 93da22ac78163dbfc9b4eb48f3696a73f1870f16
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938096"
---
# <a name="update-workposition"></a><span data-ttu-id="41043-103">Atualizar workPosition</span><span class="sxs-lookup"><span data-stu-id="41043-103">Update workPosition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41043-104">Atualiza as propriedades de um objeto [workPosition](../resources/workposition.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="41043-104">Update the properties of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="41043-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="41043-105">Permissions</span></span>

<span data-ttu-id="41043-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41043-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41043-108">Permission type</span></span>                        | <span data-ttu-id="41043-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41043-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="41043-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41043-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="41043-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="41043-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="41043-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41043-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41043-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="41043-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="41043-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41043-114">Application</span></span>                            | <span data-ttu-id="41043-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41043-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="41043-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41043-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="41043-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41043-117">Request headers</span></span>

| <span data-ttu-id="41043-118">Nome</span><span class="sxs-lookup"><span data-stu-id="41043-118">Name</span></span>           |<span data-ttu-id="41043-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="41043-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="41043-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="41043-120">Authorization</span></span>  | <span data-ttu-id="41043-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41043-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="41043-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41043-123">Content-Type</span></span>   | <span data-ttu-id="41043-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41043-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="41043-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41043-126">Request body</span></span>

<span data-ttu-id="41043-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="41043-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="41043-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="41043-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="41043-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="41043-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="41043-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41043-130">Property</span></span>     | <span data-ttu-id="41043-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="41043-131">Type</span></span>                                        | <span data-ttu-id="41043-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="41043-132">Description</span></span>                                                                                                 |
|:-------------|:--------------------------------------------|:------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="41043-133">categories</span><span class="sxs-lookup"><span data-stu-id="41043-133">categories</span></span>|<span data-ttu-id="41043-134">String collection</span><span class="sxs-lookup"><span data-stu-id="41043-134">String collection</span></span>                                | <span data-ttu-id="41043-135">Contém categorias que um usuário associou à posição.</span><span class="sxs-lookup"><span data-stu-id="41043-135">Contains categories a user has associated with the position.</span></span> <span data-ttu-id="41043-136">(por exemplo: transformação digital, MS Graph, pessoas)</span><span class="sxs-lookup"><span data-stu-id="41043-136">(eg: digital transformation, ms graph, people)</span></span> |
|<span data-ttu-id="41043-137">detalhada</span><span class="sxs-lookup"><span data-stu-id="41043-137">detail</span></span>    |[<span data-ttu-id="41043-138">positionDetail</span><span class="sxs-lookup"><span data-stu-id="41043-138">positionDetail</span></span>](../resources/positiondetail.md) | <span data-ttu-id="41043-139">Contém detalhes sobre uma posição de trabalho dos usuários.</span><span class="sxs-lookup"><span data-stu-id="41043-139">Contains detail about a users work position.</span></span>                                                                |

## <a name="response"></a><span data-ttu-id="41043-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="41043-140">Response</span></span>

<span data-ttu-id="41043-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [workPosition](../resources/workposition.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41043-141">If successful, this method returns a `200 OK` response code and an updated [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41043-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41043-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41043-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41043-143">Request</span></span>

<span data-ttu-id="41043-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41043-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_workposition"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/positions/{id}
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

### <a name="response"></a><span data-ttu-id="41043-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="41043-145">Response</span></span>

<span data-ttu-id="41043-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41043-146">The following is an example of the response.</span></span>

> <span data-ttu-id="41043-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41043-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Update workposition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
