---
title: Atualizar calendargroup
description: Atualiza as propriedades do objeto calendargroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b2b6ae3334a22cf3a98e23c9b5068d156792dc2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944579"
---
# <a name="update-calendargroup"></a><span data-ttu-id="b0240-103">Atualizar calendargroup</span><span class="sxs-lookup"><span data-stu-id="b0240-103">Update calendargroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0240-104">Atualiza as propriedades do objeto calendargroup.</span><span class="sxs-lookup"><span data-stu-id="b0240-104">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0240-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0240-105">Permissions</span></span>

<span data-ttu-id="b0240-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0240-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0240-108">Permission type</span></span>                        | <span data-ttu-id="b0240-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0240-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="b0240-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0240-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0240-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0240-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="b0240-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0240-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0240-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0240-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="b0240-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0240-114">Application</span></span>                            | <span data-ttu-id="b0240-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0240-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b0240-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0240-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="b0240-117">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b0240-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b0240-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0240-118">Request headers</span></span>

| <span data-ttu-id="b0240-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0240-119">Header</span></span>        | <span data-ttu-id="b0240-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b0240-120">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="b0240-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0240-121">Authorization</span></span> | <span data-ttu-id="b0240-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0240-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b0240-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0240-124">Content-Type</span></span>  | <span data-ttu-id="b0240-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0240-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0240-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0240-127">Request body</span></span>

<span data-ttu-id="b0240-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b0240-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b0240-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0240-131">Property</span></span> | <span data-ttu-id="b0240-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0240-132">Type</span></span>   | <span data-ttu-id="b0240-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0240-133">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="b0240-134">name</span><span class="sxs-lookup"><span data-stu-id="b0240-134">name</span></span>     | <span data-ttu-id="b0240-135">String</span><span class="sxs-lookup"><span data-stu-id="b0240-135">String</span></span> | <span data-ttu-id="b0240-136">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="b0240-136">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="b0240-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0240-137">Response</span></span>

<span data-ttu-id="b0240-138">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0240-138">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0240-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0240-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b0240-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0240-140">Request</span></span>

<span data-ttu-id="b0240-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0240-141">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b0240-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0240-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0240-143">C#</span><span class="sxs-lookup"><span data-stu-id="b0240-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0240-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0240-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0240-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b0240-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b0240-146">Java</span><span class="sxs-lookup"><span data-stu-id="b0240-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b0240-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0240-147">Response</span></span>

<span data-ttu-id="b0240-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0240-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
