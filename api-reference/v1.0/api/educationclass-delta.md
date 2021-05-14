---
title: 'educationClass: delta'
description: Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e9d1611ff27616eb825f0f27c9f7fcd5ceb8f0bd
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475020"
---
# <a name="educationclass-delta"></a><span data-ttu-id="28f61-103">educationClass: delta</span><span class="sxs-lookup"><span data-stu-id="28f61-103">educationClass: delta</span></span>

<span data-ttu-id="28f61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28f61-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28f61-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span><span class="sxs-lookup"><span data-stu-id="28f61-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="28f61-106">Consulte [Usar consulta delta para](/graph/delta-query-overview) obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="28f61-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="28f61-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="28f61-107">Permissions</span></span>

<span data-ttu-id="28f61-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28f61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28f61-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28f61-110">Permission type</span></span>                        | <span data-ttu-id="28f61-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28f61-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="28f61-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28f61-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="28f61-113">EduRoster.ReadBasic, EduRoster.Read ou EduRoster.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28f61-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="28f61-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28f61-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28f61-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28f61-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="28f61-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28f61-116">Application</span></span>                            | <span data-ttu-id="28f61-117">EduRoster.ReadBasic.All, EduRoster.Read.All ou EduRoster.WriteWrite.All</span><span class="sxs-lookup"><span data-stu-id="28f61-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28f61-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28f61-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/classes/delta
```

## <a name="request-headers"></a><span data-ttu-id="28f61-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28f61-119">Request headers</span></span>

| <span data-ttu-id="28f61-120">Nome</span><span class="sxs-lookup"><span data-stu-id="28f61-120">Name</span></span>          | <span data-ttu-id="28f61-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="28f61-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="28f61-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="28f61-122">Authorization</span></span> | <span data-ttu-id="28f61-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28f61-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28f61-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28f61-125">Request body</span></span>

<span data-ttu-id="28f61-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28f61-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28f61-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="28f61-127">Response</span></span>

<span data-ttu-id="28f61-128">Se tiver êxito, essa função retornará um código `200 OK` de resposta e uma coleção [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28f61-128">If successful, this function returns an `200 OK` response code and an [educationClass](../resources/educationclass.md) collection in the response body.</span></span> <span data-ttu-id="28f61-129">A resposta também inclui uma URL `nextLink` ou `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="28f61-129">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="28f61-130">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="28f61-130">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="28f61-131">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="28f61-131">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="28f61-132">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="28f61-132">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="28f61-133">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="28f61-133">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="28f61-134">Para obter detalhes, consulte [Using delta query](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="28f61-134">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="28f61-135">Por exemplo, solicitações, [consulte Obter alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="28f61-135">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="28f61-136">os deltas educationClass não incluem classes excluídas.</span><span class="sxs-lookup"><span data-stu-id="28f61-136">educationClass deltas do not include deleted classes.</span></span>

## <a name="examples"></a><span data-ttu-id="28f61-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="28f61-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="28f61-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28f61-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="28f61-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="28f61-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/delta
```
# <a name="c"></a>[<span data-ttu-id="28f61-140">C#</span><span class="sxs-lookup"><span data-stu-id="28f61-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28f61-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28f61-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28f61-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28f61-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28f61-143">Java</span><span class="sxs-lookup"><span data-stu-id="28f61-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationclass-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="28f61-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="28f61-144">Response</span></span>

> <span data-ttu-id="28f61-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28f61-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationClass)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{

  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationClass)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/classes/delta?$skiptoken=sU1S4IJGk3hwxbia8...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "String (identifier)",
      "displayName": "String",
      "mailNickname": "String",
      "description": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "classCode": "String",
      "externalName": "String",
      "externalId": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "grade": "String",
      "term": {
        "@odata.type": "microsoft.graph.educationTerm"
      }
    }
  ]
}
```
