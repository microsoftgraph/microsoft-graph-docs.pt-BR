---
title: Listar qualificações
description: Recupere uma lista de objetos skillProficiency.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bfaa9d5eb967391627df730c913ec805217b48e6
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937739"
---
# <a name="list-skills"></a><span data-ttu-id="1274e-103">Listar qualificações</span><span class="sxs-lookup"><span data-stu-id="1274e-103">List skills</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1274e-104">Recupere uma lista de objetos [skillProficiency](../resources/skillproficiency.md) no [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="1274e-104">Retrieve a list of [skillProficiency](../resources/skillproficiency.md) objects in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1274e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1274e-105">Permissions</span></span>

<span data-ttu-id="1274e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1274e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1274e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1274e-108">Permission type</span></span>                        | <span data-ttu-id="1274e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1274e-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="1274e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1274e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1274e-111">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1274e-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1274e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1274e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1274e-113">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1274e-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="1274e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1274e-114">Application</span></span>                            | <span data-ttu-id="1274e-115">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1274e-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="1274e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1274e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/skills
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1274e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1274e-117">Optional query parameters</span></span>

<span data-ttu-id="1274e-118">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1274e-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="1274e-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1274e-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="1274e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1274e-120">Name</span></span>            |<span data-ttu-id="1274e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1274e-121">Value</span></span>    |<span data-ttu-id="1274e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1274e-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="1274e-123">$filter</span><span class="sxs-lookup"><span data-stu-id="1274e-123">$filter</span></span>         |<span data-ttu-id="1274e-124">string</span><span class="sxs-lookup"><span data-stu-id="1274e-124">string</span></span>   |<span data-ttu-id="1274e-125">Limita a resposta somente aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="1274e-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="1274e-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="1274e-126">$orderby</span></span>        |<span data-ttu-id="1274e-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1274e-127">string</span></span>   |<span data-ttu-id="1274e-128">Por padrão, os objetos na resposta são classificados por seu valor **createdDateTime** em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="1274e-128">By default, the objects in the response are sorted by their **createdDateTime** value in a query.</span></span> <span data-ttu-id="1274e-129">Você pode alterar a ordem da resposta usando o `$orderby` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1274e-129">You can change the order of the of the response using the `$orderby` parameter.</span></span>|
|<span data-ttu-id="1274e-130">$select</span><span class="sxs-lookup"><span data-stu-id="1274e-130">$select</span></span>         |<span data-ttu-id="1274e-131">string</span><span class="sxs-lookup"><span data-stu-id="1274e-131">string</span></span>   |<span data-ttu-id="1274e-p104">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="1274e-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="1274e-134">$skip</span><span class="sxs-lookup"><span data-stu-id="1274e-134">$skip</span></span>           |<span data-ttu-id="1274e-135">int</span><span class="sxs-lookup"><span data-stu-id="1274e-135">int</span></span>      |<span data-ttu-id="1274e-136">Ignore os primeiros n resultados, útil para paginação.</span><span class="sxs-lookup"><span data-stu-id="1274e-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="1274e-137">$top</span><span class="sxs-lookup"><span data-stu-id="1274e-137">$top</span></span>            |<span data-ttu-id="1274e-138">int</span><span class="sxs-lookup"><span data-stu-id="1274e-138">int</span></span>      |<span data-ttu-id="1274e-139">Número de resultados a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="1274e-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="1274e-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1274e-140">Request headers</span></span>

| <span data-ttu-id="1274e-141">Nome</span><span class="sxs-lookup"><span data-stu-id="1274e-141">Name</span></span>           |<span data-ttu-id="1274e-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="1274e-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="1274e-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="1274e-143">Authorization</span></span>  | <span data-ttu-id="1274e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1274e-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1274e-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1274e-146">Content-Type</span></span>   | <span data-ttu-id="1274e-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1274e-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1274e-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1274e-149">Request body</span></span>

<span data-ttu-id="1274e-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1274e-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1274e-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="1274e-151">Response</span></span>

<span data-ttu-id="1274e-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [skillProficiency](../resources/skillproficiency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1274e-152">If successful, this method returns a `200 OK` response code and a collection of [skillProficiency](../resources/skillproficiency.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1274e-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1274e-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1274e-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1274e-154">Request</span></span>

<span data-ttu-id="1274e-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1274e-155">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_skills"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/skills
```

### <a name="response"></a><span data-ttu-id="1274e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="1274e-156">Response</span></span>

<span data-ttu-id="1274e-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1274e-157">The following is an example of the response.</span></span>

> <span data-ttu-id="1274e-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1274e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "categories": [
        "categories-value"
      ],
      "displayName": "displayName-value",
      "proficiency": "proficiency-value",
      "webUrl": "webUrl-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List skills",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
