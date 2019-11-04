---
title: Listar nomes
description: Recupere uma lista de objetos PersonName do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5c13b3ee7454c8b8f0061aafbd9d0bebea6da94a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937767"
---
# <a name="list-names"></a><span data-ttu-id="caca2-103">Listar nomes</span><span class="sxs-lookup"><span data-stu-id="caca2-103">List names</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caca2-104">Recupere uma lista de objetos [PersonName](../resources/personname.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="caca2-104">Retrieve a list of [personName](../resources/personname.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="caca2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="caca2-105">Permissions</span></span>

<span data-ttu-id="caca2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caca2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="caca2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caca2-108">Permission type</span></span>                        | <span data-ttu-id="caca2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="caca2-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="caca2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caca2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="caca2-111">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="caca2-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="caca2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caca2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caca2-113">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="caca2-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="caca2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caca2-114">Application</span></span>                            | <span data-ttu-id="caca2-115">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="caca2-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="caca2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="caca2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names
```

## <a name="optional-query-parameters"></a><span data-ttu-id="caca2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="caca2-117">Optional query parameters</span></span>

<span data-ttu-id="caca2-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="caca2-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="caca2-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="caca2-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="caca2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="caca2-120">Request headers</span></span>

| <span data-ttu-id="caca2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="caca2-121">Name</span></span>           |<span data-ttu-id="caca2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="caca2-122">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="caca2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="caca2-123">Authorization</span></span>  | <span data-ttu-id="caca2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="caca2-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="caca2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="caca2-126">Content-Type</span></span>   | <span data-ttu-id="caca2-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="caca2-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="caca2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="caca2-129">Request body</span></span> 

<span data-ttu-id="caca2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="caca2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="caca2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="caca2-131">Response</span></span>

<span data-ttu-id="caca2-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [PersonName](../resources/personname.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="caca2-132">If successful, this method returns a `200 OK` response code and a collection of [personName](../resources/personname.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="caca2-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="caca2-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="caca2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="caca2-134">Request</span></span>

<span data-ttu-id="caca2-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="caca2-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/names
```

### <a name="response"></a><span data-ttu-id="caca2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="caca2-136">Response</span></span>

<span data-ttu-id="caca2-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="caca2-137">The following is an example of the response.</span></span>

> <span data-ttu-id="caca2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="caca2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "first": "first-value",
      "initials": "initials-value",
      "last": "last-value",
      "languageTag": "languageTag-value",
      "maiden": "maiden-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List names",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->