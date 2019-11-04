---
title: Atualizar educationalactivity
description: Atualiza as propriedades de um objeto educationalactivity.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 3a4b792803065dc7f2f9567873e81ec369a33f66
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938082"
---
# <a name="update-educationalactivity"></a><span data-ttu-id="f95c4-103">Atualizar educationalactivity</span><span class="sxs-lookup"><span data-stu-id="f95c4-103">Update educationalactivity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f95c4-104">Atualizar as propriedades de um objeto [educationalActivity](../resources/educationalactivity.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f95c4-104">Update the properties of an [educationalActivity](../resources/educationalactivity.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f95c4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f95c4-105">Permissions</span></span>

<span data-ttu-id="f95c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f95c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f95c4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f95c4-108">Permission type</span></span>                        | <span data-ttu-id="f95c4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f95c4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f95c4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f95c4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f95c4-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f95c4-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f95c4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f95c4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f95c4-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f95c4-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="f95c4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f95c4-114">Application</span></span>                            | <span data-ttu-id="f95c4-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f95c4-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="f95c4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f95c4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/educationalActivities/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="f95c4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f95c4-117">Request headers</span></span>

| <span data-ttu-id="f95c4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f95c4-118">Name</span></span>           |<span data-ttu-id="f95c4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f95c4-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="f95c4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f95c4-120">Authorization</span></span>  | <span data-ttu-id="f95c4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f95c4-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f95c4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f95c4-123">Content-Type</span></span>   | <span data-ttu-id="f95c4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f95c4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f95c4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f95c4-126">Request body</span></span>

<span data-ttu-id="f95c4-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f95c4-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f95c4-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f95c4-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f95c4-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f95c4-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f95c4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f95c4-130">Property</span></span>           | <span data-ttu-id="f95c4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f95c4-131">Type</span></span>                                                                  | <span data-ttu-id="f95c4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f95c4-132">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="f95c4-133">completionMonthYear</span><span class="sxs-lookup"><span data-stu-id="f95c4-133">completionMonthYear</span></span> |<span data-ttu-id="f95c4-134">Data</span><span class="sxs-lookup"><span data-stu-id="f95c4-134">Date</span></span>                                                                   | <span data-ttu-id="f95c4-135">O mês e o ano em que o usuário formou ou concluiu a atividade.</span><span class="sxs-lookup"><span data-stu-id="f95c4-135">The month and year the user graduated or completed the activity.</span></span>           |
|<span data-ttu-id="f95c4-136">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="f95c4-136">endMonthYear</span></span>        |<span data-ttu-id="f95c4-137">Data</span><span class="sxs-lookup"><span data-stu-id="f95c4-137">Date</span></span>                                                                   | <span data-ttu-id="f95c4-138">O mês e o ano em que o usuário concluiu a atividade educacional referenciada.</span><span class="sxs-lookup"><span data-stu-id="f95c4-138">The month and year the user completed the educational activity referenced.</span></span> |
|<span data-ttu-id="f95c4-139">instituição</span><span class="sxs-lookup"><span data-stu-id="f95c4-139">institution</span></span>         |[<span data-ttu-id="f95c4-140">institutionData</span><span class="sxs-lookup"><span data-stu-id="f95c4-140">institutionData</span></span>](../resources/institutiondata.md)                     | <span data-ttu-id="f95c4-141">Contém detalhes da instituição estudada em.</span><span class="sxs-lookup"><span data-stu-id="f95c4-141">Contains details of the institution studied at.</span></span>                            |
|<span data-ttu-id="f95c4-142">programa</span><span class="sxs-lookup"><span data-stu-id="f95c4-142">program</span></span>             |[<span data-ttu-id="f95c4-143">educationalActivityDetail</span><span class="sxs-lookup"><span data-stu-id="f95c4-143">educationalActivityDetail</span></span>](../resources/educationalactivitydetail.md) | <span data-ttu-id="f95c4-144">Contém informações estendidas sobre o programa ou o curso.</span><span class="sxs-lookup"><span data-stu-id="f95c4-144">Contains extended information about the program or course.</span></span>                 |
|<span data-ttu-id="f95c4-145">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="f95c4-145">startMonthYear</span></span>      |<span data-ttu-id="f95c4-146">Data</span><span class="sxs-lookup"><span data-stu-id="f95c4-146">Date</span></span>                                                                   | <span data-ttu-id="f95c4-147">O mês e o ano em que o usuário tiver iniciado a atividade referenciada.</span><span class="sxs-lookup"><span data-stu-id="f95c4-147">The month and year the user commenced the activity referenced.</span></span>             |

## <a name="response"></a><span data-ttu-id="f95c4-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f95c4-148">Response</span></span>

<span data-ttu-id="f95c4-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationalActivity](../resources/educationalactivity.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f95c4-149">If successful, this method returns a `200 OK` response code and an updated [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f95c4-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f95c4-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f95c4-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f95c4-151">Request</span></span>

<span data-ttu-id="f95c4-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f95c4-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationalactivity"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/educationalActivities/{id}
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

### <a name="response"></a><span data-ttu-id="f95c4-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f95c4-153">Response</span></span>

<span data-ttu-id="f95c4-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f95c4-154">The following is an example of the response.</span></span>

> <span data-ttu-id="f95c4-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f95c4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Update educationalactivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->