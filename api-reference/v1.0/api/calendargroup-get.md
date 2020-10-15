---
title: Obter calendarGroup
description: Recupera as propriedades e os relacionamentos de um objeto de grupo de calendários.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 673cfd54f22912ba593abc4d5e72dd42c80020c6
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459890"
---
# <a name="get-calendargroup"></a><span data-ttu-id="64477-103">Obter calendarGroup</span><span class="sxs-lookup"><span data-stu-id="64477-103">Get calendarGroup</span></span>

<span data-ttu-id="64477-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64477-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64477-105">Recupera as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="64477-105">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64477-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="64477-106">Permissions</span></span>

<span data-ttu-id="64477-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64477-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64477-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64477-109">Permission type</span></span>                        | <span data-ttu-id="64477-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64477-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="64477-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64477-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="64477-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="64477-112">Calendars.Read</span></span>                              |
| <span data-ttu-id="64477-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64477-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64477-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="64477-114">Calendars.Read</span></span>                              |
| <span data-ttu-id="64477-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64477-115">Application</span></span>                            | <span data-ttu-id="64477-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="64477-116">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="64477-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64477-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="64477-118">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="64477-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64477-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64477-119">Optional query parameters</span></span>

<span data-ttu-id="64477-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="64477-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64477-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64477-121">Request headers</span></span>

| <span data-ttu-id="64477-122">Nome</span><span class="sxs-lookup"><span data-stu-id="64477-122">Name</span></span>          | <span data-ttu-id="64477-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="64477-123">Type</span></span>   | <span data-ttu-id="64477-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="64477-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="64477-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="64477-125">Authorization</span></span> | <span data-ttu-id="64477-126">string</span><span class="sxs-lookup"><span data-stu-id="64477-126">string</span></span> | <span data-ttu-id="64477-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64477-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64477-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64477-129">Request body</span></span>

<span data-ttu-id="64477-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64477-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64477-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="64477-131">Response</span></span>

<span data-ttu-id="64477-132">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64477-132">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64477-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64477-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="64477-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64477-134">Request</span></span>

<span data-ttu-id="64477-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64477-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="64477-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="64477-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="64477-137">C#</span><span class="sxs-lookup"><span data-stu-id="64477-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64477-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64477-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64477-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64477-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64477-140">Java</span><span class="sxs-lookup"><span data-stu-id="64477-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="64477-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="64477-141">Response</span></span>

<span data-ttu-id="64477-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64477-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
