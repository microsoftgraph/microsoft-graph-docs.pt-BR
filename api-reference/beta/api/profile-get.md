---
title: Obter perfil
description: Recupere as propriedades e os relacionamentos do objeto de perfil.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fd6c68f79ffb417b12eb1f8e28d874f4461fb24e
ms.sourcegitcommit: 5d4bf35774eba6de21f4252b46f7e9d8f64a517f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/08/2020
ms.locfileid: "44168553"
---
# <a name="get-profile"></a><span data-ttu-id="ea3a9-103">Obter perfil</span><span class="sxs-lookup"><span data-stu-id="ea3a9-103">Get profile</span></span>

<span data-ttu-id="ea3a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea3a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea3a9-105">Recupere as propriedades e os relacionamentos de um objeto de [perfil](../resources/profile.md) para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-105">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

<span data-ttu-id="ea3a9-106">O recurso de **perfil** expõe várias propriedades sofisticadas que são descritivas do usuário como [relações](../resources/profile.md#relationships), por exemplo, aniversários e atividades de educação.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-106">The **profile** resource exposes various rich properties that are descriptive of the user as [relationships](../resources/profile.md#relationships), for example, anniversaries and education activities.</span></span> <span data-ttu-id="ea3a9-107">Para obter uma destas propriedades de navegação, use o método GET correspondente nessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-107">To get one of these navigation properties, use the corresponding GET method on that property.</span></span> <span data-ttu-id="ea3a9-108">Consulte os [métodos](../resources/profile.md) expostos por **perfil**.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-108">See the [methods](../resources/profile.md) exposed by **profile**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea3a9-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea3a9-109">Permissions</span></span>

<span data-ttu-id="ea3a9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea3a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea3a9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea3a9-112">Permission type</span></span>                        | <span data-ttu-id="ea3a9-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea3a9-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ea3a9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea3a9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea3a9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-115">Not supported.</span></span>                              |
| <span data-ttu-id="ea3a9-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea3a9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea3a9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-117">Not supported.</span></span>                              |
| <span data-ttu-id="ea3a9-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea3a9-118">Application</span></span>                            | <span data-ttu-id="ea3a9-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-119">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="ea3a9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea3a9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea3a9-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ea3a9-121">Optional query parameters</span></span>

<span data-ttu-id="ea3a9-122">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ea3a9-123">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ea3a9-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea3a9-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea3a9-124">Request headers</span></span>

| <span data-ttu-id="ea3a9-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ea3a9-125">Name</span></span>           |<span data-ttu-id="ea3a9-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea3a9-126">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="ea3a9-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea3a9-127">Authorization</span></span>  | <span data-ttu-id="ea3a9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ea3a9-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea3a9-130">Content-Type</span></span>   | <span data-ttu-id="ea3a9-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea3a9-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea3a9-133">Request body</span></span>

<span data-ttu-id="ea3a9-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea3a9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea3a9-135">Response</span></span>

<span data-ttu-id="ea3a9-136">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto de [perfil](../resources/profile.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-136">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ea3a9-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ea3a9-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ea3a9-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea3a9-138">Request</span></span>

<span data-ttu-id="ea3a9-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea3a9-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea3a9-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile
```
# <a name="c"></a>[<span data-ttu-id="ea3a9-141">C#</span><span class="sxs-lookup"><span data-stu-id="ea3a9-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea3a9-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea3a9-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea3a9-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea3a9-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ea3a9-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea3a9-144">Response</span></span>

<span data-ttu-id="ea3a9-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-145">The following is an example of the response.</span></span>

> <span data-ttu-id="ea3a9-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea3a9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get profile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
