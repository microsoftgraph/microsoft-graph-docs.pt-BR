---
title: 'Planejador: delta'
description: Recupera as alterações em objetos que o usuário está inscrito em.
author: TarkanSevilmis
ms.openlocfilehash: dcc60ad9c1bc5ea9e56099d4bc79fb57d4e95374
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323363"
---
# <a name="planner-delta"></a><span data-ttu-id="c0ceb-103">Planejador: delta</span><span class="sxs-lookup"><span data-stu-id="c0ceb-103">Planner: delta</span></span>

> <span data-ttu-id="c0ceb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0ceb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0ceb-106">Recupera as alterações em objetos que o usuário está [inscrito](../resources/planner-overview.md#track-changes-using-delta-query) .</span><span class="sxs-lookup"><span data-stu-id="c0ceb-106">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="c0ceb-107">Esse método permite que o seu aplicativo para controlar as alterações nos objetos que o usuário pode acessar dentro Planejador ao longo do tempo.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-107">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="c0ceb-108">O valor de retorno deste método deve conter heterogêneo tipos de objetos do planejador.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-108">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="c0ceb-109">Para obter mais informações sobre o controle de alterações nos dados do Microsoft Graph, consulte [consulta delta de usar para rastrear alterações nos dados do Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="c0ceb-109">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0ceb-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0ceb-110">Permissions</span></span>

<span data-ttu-id="c0ceb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0ceb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0ceb-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0ceb-113">Permission type</span></span>      | <span data-ttu-id="c0ceb-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0ceb-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0ceb-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0ceb-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c0ceb-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0ceb-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c0ceb-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0ceb-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0ceb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-118">Not supported.</span></span>    |
|<span data-ttu-id="c0ceb-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0ceb-119">Application</span></span> | <span data-ttu-id="c0ceb-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0ceb-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0ceb-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/<id>/planner/all/delta
```

<span data-ttu-id="c0ceb-122">Sem parâmetros de consulta adicionais (como `$select`, `$expand`, ou `$filter`) são suportados atualmente na implementação do Planejador de consultas delta.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-122">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0ceb-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0ceb-123">Request headers</span></span>

| <span data-ttu-id="c0ceb-124">Nome</span><span class="sxs-lookup"><span data-stu-id="c0ceb-124">Name</span></span>           |<span data-ttu-id="c0ceb-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0ceb-125">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="c0ceb-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0ceb-126">Authorization</span></span>  | <span data-ttu-id="c0ceb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0ceb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0ceb-129">Request body</span></span>

<span data-ttu-id="c0ceb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0ceb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0ceb-131">Response</span></span>

<span data-ttu-id="c0ceb-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um conjunto de alterações a serem aplicadas a objetos no corpo da resposta e um link de sincronização Delta a seguir.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-132">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="c0ceb-133">Se o `deltaLink` que usa o chamador é mal formados, esse ponto de extremidade retornará HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-133">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="c0ceb-134">Se o `deltaLink` que usa o chamador é muito antigo, esse ponto de extremidade retornará 410 HTTP.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-134">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="c0ceb-p104">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c0ceb-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c0ceb-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0ceb-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c0ceb-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0ceb-139">Request</span></span>

<span data-ttu-id="c0ceb-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-140">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```http
GET https://graph.microsoft.com/beta/me/planner/all/delta
```

##### <a name="response"></a><span data-ttu-id="c0ceb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0ceb-141">Response</span></span>
<span data-ttu-id="c0ceb-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-142">Here is an example of the response.</span></span>

><span data-ttu-id="c0ceb-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-143">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="c0ceb-144">Todas as propriedades alteradas serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0ceb-144">All the changed properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List changes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
