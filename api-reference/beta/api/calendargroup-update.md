---
title: Atualizar calendargroup
description: Atualiza as propriedades do objeto calendargroup.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: aa4326f1a4bdd71531dd41cbd206c6f5365f76cb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987544"
---
# <a name="update-calendargroup"></a><span data-ttu-id="34db9-103">Atualizar calendargroup</span><span class="sxs-lookup"><span data-stu-id="34db9-103">Update calendargroup</span></span>

<span data-ttu-id="34db9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34db9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34db9-105">Atualiza as propriedades do objeto calendargroup.</span><span class="sxs-lookup"><span data-stu-id="34db9-105">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="34db9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="34db9-106">Permissions</span></span>

<span data-ttu-id="34db9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34db9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34db9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34db9-109">Permission type</span></span>                        | <span data-ttu-id="34db9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34db9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="34db9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34db9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="34db9-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34db9-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="34db9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34db9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34db9-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34db9-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="34db9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34db9-115">Application</span></span>                            | <span data-ttu-id="34db9-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34db9-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="34db9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34db9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="34db9-118">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="34db9-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="34db9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34db9-119">Request headers</span></span>

| <span data-ttu-id="34db9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34db9-120">Header</span></span>        | <span data-ttu-id="34db9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="34db9-121">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="34db9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34db9-122">Authorization</span></span> | <span data-ttu-id="34db9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34db9-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="34db9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34db9-125">Content-Type</span></span>  | <span data-ttu-id="34db9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34db9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34db9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34db9-128">Request body</span></span>

<span data-ttu-id="34db9-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="34db9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="34db9-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34db9-132">Property</span></span> | <span data-ttu-id="34db9-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="34db9-133">Type</span></span>   | <span data-ttu-id="34db9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="34db9-134">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="34db9-135">nome</span><span class="sxs-lookup"><span data-stu-id="34db9-135">name</span></span>     | <span data-ttu-id="34db9-136">String</span><span class="sxs-lookup"><span data-stu-id="34db9-136">String</span></span> | <span data-ttu-id="34db9-137">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="34db9-137">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="34db9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="34db9-138">Response</span></span>

<span data-ttu-id="34db9-139">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34db9-139">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34db9-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34db9-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="34db9-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34db9-141">Request</span></span>

<span data-ttu-id="34db9-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34db9-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="34db9-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="34db9-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="34db9-144">C#</span><span class="sxs-lookup"><span data-stu-id="34db9-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34db9-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34db9-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34db9-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34db9-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="34db9-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="34db9-147">Response</span></span>

<span data-ttu-id="34db9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34db9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


