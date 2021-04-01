---
title: 'Planner: delta'
description: Recupera as alterações nos objetos aos que o usuário está inscrito.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 7c730630f3fd655db29c93c699e8090d3046a4d4
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473490"
---
# <a name="planner-delta"></a><span data-ttu-id="d6101-103">Planner: delta</span><span class="sxs-lookup"><span data-stu-id="d6101-103">Planner: delta</span></span>

<span data-ttu-id="d6101-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6101-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6101-105">Recupera as alterações nos objetos aos que o usuário [está inscrito.](../resources/planner-overview.md#track-changes-using-delta-query)</span><span class="sxs-lookup"><span data-stu-id="d6101-105">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="d6101-106">Esse método permite que seu aplicativo acompanhe as alterações nos objetos que o usuário pode acessar no Planner ao longo do tempo.</span><span class="sxs-lookup"><span data-stu-id="d6101-106">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="d6101-107">O valor de retorno desse método pode conter tipos hetergêneos de objetos do Planner.</span><span class="sxs-lookup"><span data-stu-id="d6101-107">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="d6101-108">Para obter mais informações sobre o controle de alterações nos dados do Microsoft Graph, consulte [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="d6101-108">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6101-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6101-109">Permissions</span></span>

<span data-ttu-id="d6101-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6101-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6101-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6101-112">Permission type</span></span>      | <span data-ttu-id="d6101-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6101-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6101-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6101-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d6101-115">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6101-115">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6101-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6101-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6101-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6101-117">Not supported.</span></span>    |
|<span data-ttu-id="d6101-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6101-118">Application</span></span> | <span data-ttu-id="d6101-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6101-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6101-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6101-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/{id}/planner/all/delta
```

<span data-ttu-id="d6101-121">No momento, não há suporte para parâmetros de consulta adicionais (como , ou ) na implementação de consultas `$select` `$expand` delta do `$filter` Planner.</span><span class="sxs-lookup"><span data-stu-id="d6101-121">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6101-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6101-122">Request headers</span></span>

| <span data-ttu-id="d6101-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d6101-123">Name</span></span>           |<span data-ttu-id="d6101-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6101-124">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="d6101-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6101-125">Authorization</span></span>  | <span data-ttu-id="d6101-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6101-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6101-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6101-128">Request body</span></span>

<span data-ttu-id="d6101-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6101-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6101-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6101-130">Response</span></span>

<span data-ttu-id="d6101-131">Se tiver êxito, este método retornará um código de resposta e uma coleção de alterações a serem aplicadas a objetos no corpo da resposta e um link de Sincronização `200 OK` Delta a ser seguido.</span><span class="sxs-lookup"><span data-stu-id="d6101-131">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="d6101-132">Se o `deltaLink` que o chamador usa estiver malformado, esse ponto de extremidade retornará HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="d6101-132">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="d6101-133">Se o `deltaLink` que o chamador usa for muito antigo, esse ponto de extremidade retornará HTTP 410.</span><span class="sxs-lookup"><span data-stu-id="d6101-133">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="d6101-134">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="d6101-134">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="d6101-135">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="d6101-135">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="d6101-136">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d6101-136">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d6101-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6101-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d6101-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6101-138">Request</span></span>

<span data-ttu-id="d6101-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6101-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d6101-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6101-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/all/delta
```
# <a name="c"></a>[<span data-ttu-id="d6101-141">C#</span><span class="sxs-lookup"><span data-stu-id="d6101-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6101-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6101-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6101-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6101-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6101-144">Java</span><span class="sxs-lookup"><span data-stu-id="d6101-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d6101-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6101-145">Response</span></span>
<span data-ttu-id="d6101-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6101-146">Here is an example of the response.</span></span>

><span data-ttu-id="d6101-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d6101-147">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="d6101-148">Todas as propriedades alteradas serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6101-148">All the changed properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_delta",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.entity)",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
cache-control: private
client-request-id: 3acb384b-e2d1-4a46-a347-e03bc6428cac
request-id: 3acb384b-e2d1-4a46-a347-e03bc6428cac
preference-applied: odata.track-changes, odata.track-changes

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.plannerDelta)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/me/planner/all/delta?$deltatoken=jVztGMFnm7qLEQ69FaXzWF5sPEJZU2YxZa32QEvnZTZ4q4C10ThM5uL7bEPm9ysqrxOY0QQIb4Uqmc9DH3rn7pczamvtCipDVJ4FivXh398.J9pSVKpytlutvx03-iBmO4ZM_3qPztOq2T9VIjHoRR0",
    "value": [
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBASCc=\"",
            "percentComplete": 100,
            "completedDateTime": "2018-03-13T21:31:25.778Z",
            "completedBy": {
                "user": {
                    "id": "8414b634-316f-41ba-b6a6-646a2949e3a5"
                }
            },
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        },
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBATCc=\"",
            "percentComplete": 0,
            "completedDateTime": null,
            "completedBy": null,
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        },
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAUCc=\"",
            "title": "Title change",
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List changes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


