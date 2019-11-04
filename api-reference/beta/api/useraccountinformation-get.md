---
title: Obter userAccountInformation
description: Recupere as propriedades e os relacionamentos do objeto useraccountinformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: Profile
doc_type: apiPageType
ms.openlocfilehash: a13208654b343fdff29b2495c58ebc54a168b52e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937452"
---
# <a name="get-useraccountinformation"></a><span data-ttu-id="c0782-103">Obter userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="c0782-103">Get userAccountInformation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0782-104">Recupere as propriedades e os relacionamentos de um objeto [userAccountInformation](../resources/useraccountinformation.md) .</span><span class="sxs-lookup"><span data-stu-id="c0782-104">Retrieve the properties and relationships of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0782-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0782-105">Permissions</span></span>

<span data-ttu-id="c0782-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0782-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0782-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0782-108">Permission type</span></span>                        | <span data-ttu-id="c0782-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0782-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c0782-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0782-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0782-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0782-111">Not supported.</span></span> |
| <span data-ttu-id="c0782-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0782-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0782-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0782-113">Not supported.</span></span> |
| <span data-ttu-id="c0782-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0782-114">Application</span></span>                            | <span data-ttu-id="c0782-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0782-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0782-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0782-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /user/profile/account
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0782-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c0782-117">Optional query parameters</span></span>

<span data-ttu-id="c0782-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c0782-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c0782-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c0782-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0782-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0782-120">Request headers</span></span>

| <span data-ttu-id="c0782-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c0782-121">Name</span></span>      |<span data-ttu-id="c0782-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0782-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0782-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0782-123">Authorization</span></span> | <span data-ttu-id="c0782-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0782-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0782-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0782-126">Request body</span></span>

<span data-ttu-id="c0782-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0782-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0782-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0782-128">Response</span></span>

<span data-ttu-id="c0782-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [userAccountInformation](../resources/useraccountinformation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0782-129">If successful, this method returns a `200 OK` response code and the requested [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0782-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c0782-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c0782-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0782-131">Request</span></span>

<span data-ttu-id="c0782-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0782-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}-->

```http
GET https://graph.microsoft.com/Beta/user/profile/account
```

### <a name="response"></a><span data-ttu-id="c0782-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0782-133">Response</span></span>

<span data-ttu-id="c0782-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c0782-134">The following is an example of the response.</span></span>

> <span data-ttu-id="c0782-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0782-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get userAccountInformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
