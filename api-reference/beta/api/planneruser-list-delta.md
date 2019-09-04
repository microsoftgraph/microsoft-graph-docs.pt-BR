---
title: 'Planner: Delta'
description: Recupera alterações nos objetos nos quais o usuário está inscrito.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 57ab397437648ee1c6d0c4779e26ea19d1f5cde2
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725630"
---
# <a name="planner-delta"></a><span data-ttu-id="5463e-103">Planner: Delta</span><span class="sxs-lookup"><span data-stu-id="5463e-103">Planner: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5463e-104">Recupera alterações nos objetos nos quais o usuário está [inscrito](../resources/planner-overview.md#track-changes-using-delta-query) .</span><span class="sxs-lookup"><span data-stu-id="5463e-104">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="5463e-105">Este método permite que seu aplicativo rastreie alterações para objetos que o usuário pode acessar no planejador ao longo do tempo.</span><span class="sxs-lookup"><span data-stu-id="5463e-105">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="5463e-106">O valor de retorno desse método pode conter tipos heterogêneo de objetos do Planner.</span><span class="sxs-lookup"><span data-stu-id="5463e-106">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="5463e-107">Para obter mais informações sobre o controle de alterações nos dados do Microsoft Graph, consulte [usar a consulta Delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="5463e-107">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="5463e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5463e-108">Permissions</span></span>

<span data-ttu-id="5463e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5463e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5463e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5463e-111">Permission type</span></span>      | <span data-ttu-id="5463e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5463e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5463e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5463e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5463e-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5463e-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5463e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5463e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5463e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5463e-116">Not supported.</span></span>    |
|<span data-ttu-id="5463e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5463e-117">Application</span></span> | <span data-ttu-id="5463e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5463e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5463e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5463e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/{id}/planner/all/delta
```

<span data-ttu-id="5463e-120">Nenhum parâmetro de consulta adicional (como `$select`, `$expand`ou `$filter`) é suportado atualmente na implementação do Planner de consultas Delta.</span><span class="sxs-lookup"><span data-stu-id="5463e-120">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5463e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5463e-121">Request headers</span></span>

| <span data-ttu-id="5463e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5463e-122">Name</span></span>           |<span data-ttu-id="5463e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5463e-123">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="5463e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5463e-124">Authorization</span></span>  | <span data-ttu-id="5463e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5463e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5463e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5463e-127">Request body</span></span>

<span data-ttu-id="5463e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5463e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5463e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5463e-129">Response</span></span>

<span data-ttu-id="5463e-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de alterações a serem aplicadas aos objetos no corpo da resposta e um link de sincronização Delta a seguir.</span><span class="sxs-lookup"><span data-stu-id="5463e-130">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="5463e-131">Se o `deltaLink` chamador usa estiver malformado, este ponto de extremidade retornará http 400.</span><span class="sxs-lookup"><span data-stu-id="5463e-131">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="5463e-132">Se o `deltaLink` chamador usar for muito antigo, esse ponto de extremidade retornará http 410.</span><span class="sxs-lookup"><span data-stu-id="5463e-132">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="5463e-133">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="5463e-133">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="5463e-134">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="5463e-134">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="5463e-135">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="5463e-135">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="5463e-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5463e-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5463e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5463e-137">Request</span></span>

<span data-ttu-id="5463e-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5463e-138">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5463e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5463e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/all/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5463e-140">C#</span><span class="sxs-lookup"><span data-stu-id="5463e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5463e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5463e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5463e-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5463e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5463e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5463e-143">Response</span></span>
<span data-ttu-id="5463e-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5463e-144">Here is an example of the response.</span></span>

><span data-ttu-id="5463e-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5463e-145">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="5463e-146">Todas as propriedades alteradas serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5463e-146">All the changed properties will be returned from an actual call.</span></span>

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
