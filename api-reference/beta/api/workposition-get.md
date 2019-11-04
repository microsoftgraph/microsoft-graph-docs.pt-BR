---
title: Obter workPosition
description: Recupere as propriedades e os relacionamentos de um objeto workPosition.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e92dbe050624934947310dede69a35757caa94d2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937424"
---
# <a name="get-workposition"></a><span data-ttu-id="4eb4e-103">Obter workPosition</span><span class="sxs-lookup"><span data-stu-id="4eb4e-103">Get workPosition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eb4e-104">Recupere as propriedades e os relacionamentos de um objeto [workPosition](../resources/workposition.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-104">Retrieve the properties and relationships of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4eb4e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4eb4e-105">Permissions</span></span>

<span data-ttu-id="4eb4e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eb4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4eb4e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4eb4e-108">Permission type</span></span>                        | <span data-ttu-id="4eb4e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4eb4e-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="4eb4e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4eb4e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4eb4e-111">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4eb4e-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4eb4e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4eb4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eb4e-113">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4eb4e-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4eb4e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4eb4e-114">Application</span></span>                            | <span data-ttu-id="4eb4e-115">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4eb4e-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="4eb4e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4eb4e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/positions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4eb4e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4eb4e-117">Optional query parameters</span></span>

<span data-ttu-id="4eb4e-118">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="4eb4e-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4eb4e-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="4eb4e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4eb4e-120">Name</span></span>            |<span data-ttu-id="4eb4e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4eb4e-121">Value</span></span>    |<span data-ttu-id="4eb4e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eb4e-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4eb4e-123">$filter</span><span class="sxs-lookup"><span data-stu-id="4eb4e-123">$filter</span></span>         |<span data-ttu-id="4eb4e-124">string</span><span class="sxs-lookup"><span data-stu-id="4eb4e-124">string</span></span>   |<span data-ttu-id="4eb4e-125">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="4eb4e-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="4eb4e-126">$orderby</span></span>        |<span data-ttu-id="4eb4e-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4eb4e-127">string</span></span>   |<span data-ttu-id="4eb4e-128">Por padrão, os objetos na resposta são classificados por seu valor **createdDateTime** em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-128">By default, the objects in the response are sorted by their **createdDateTime** value in a query.</span></span> <span data-ttu-id="4eb4e-129">Você pode alterar a ordem da resposta usando o `$orderby` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-129">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="4eb4e-130">$select</span><span class="sxs-lookup"><span data-stu-id="4eb4e-130">$select</span></span>         |<span data-ttu-id="4eb4e-131">string</span><span class="sxs-lookup"><span data-stu-id="4eb4e-131">string</span></span>   |<span data-ttu-id="4eb4e-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="4eb4e-134">$skip</span><span class="sxs-lookup"><span data-stu-id="4eb4e-134">$skip</span></span>           |<span data-ttu-id="4eb4e-135">int</span><span class="sxs-lookup"><span data-stu-id="4eb4e-135">int</span></span>      |<span data-ttu-id="4eb4e-136">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="4eb4e-137">$top</span><span class="sxs-lookup"><span data-stu-id="4eb4e-137">$top</span></span>            |<span data-ttu-id="4eb4e-138">int</span><span class="sxs-lookup"><span data-stu-id="4eb4e-138">int</span></span>      |<span data-ttu-id="4eb4e-139">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="4eb4e-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4eb4e-140">Request headers</span></span>

| <span data-ttu-id="4eb4e-141">Nome</span><span class="sxs-lookup"><span data-stu-id="4eb4e-141">Name</span></span>           |<span data-ttu-id="4eb4e-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eb4e-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="4eb4e-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="4eb4e-143">Authorization</span></span>  | <span data-ttu-id="4eb4e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-p105">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="4eb4e-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4eb4e-146">Request body</span></span>

<span data-ttu-id="4eb4e-147">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eb4e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4eb4e-148">Response</span></span>

<span data-ttu-id="4eb4e-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [workPosition](../resources/workposition.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-149">If successful, this method returns a `200 OK` response code and the requested [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4eb4e-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4eb4e-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4eb4e-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4eb4e-151">Request</span></span>

<span data-ttu-id="4eb4e-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workposition"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/positions/{id}
```

### <a name="response"></a><span data-ttu-id="4eb4e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="4eb4e-153">Response</span></span>

<span data-ttu-id="4eb4e-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-154">The following is an example of the response.</span></span>

> <span data-ttu-id="4eb4e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4eb4e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Get workPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
