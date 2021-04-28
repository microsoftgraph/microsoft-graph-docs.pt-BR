---
title: Atualizar calendargroup
description: Atualiza as propriedades do objeto calendargroup.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a8b8a82010a5fb7d5a1423aa3bed8ff15645a678
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039913"
---
# <a name="update-calendargroup"></a><span data-ttu-id="5a971-103">Atualizar calendargroup</span><span class="sxs-lookup"><span data-stu-id="5a971-103">Update calendargroup</span></span>

<span data-ttu-id="5a971-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a971-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a971-105">Atualiza as propriedades do objeto calendargroup.</span><span class="sxs-lookup"><span data-stu-id="5a971-105">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a971-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a971-106">Permissions</span></span>

<span data-ttu-id="5a971-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a971-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a971-109">Permission type</span></span>                        | <span data-ttu-id="5a971-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a971-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5a971-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a971-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a971-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a971-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="5a971-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a971-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a971-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a971-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="5a971-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a971-115">Application</span></span>                            | <span data-ttu-id="5a971-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a971-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5a971-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a971-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="5a971-118">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5a971-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5a971-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a971-119">Request headers</span></span>

| <span data-ttu-id="5a971-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a971-120">Header</span></span>        | <span data-ttu-id="5a971-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5a971-121">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="5a971-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a971-122">Authorization</span></span> | <span data-ttu-id="5a971-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a971-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5a971-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a971-125">Content-Type</span></span>  | <span data-ttu-id="5a971-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a971-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a971-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a971-128">Request body</span></span>

<span data-ttu-id="5a971-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5a971-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5a971-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a971-132">Property</span></span> | <span data-ttu-id="5a971-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a971-133">Type</span></span>   | <span data-ttu-id="5a971-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a971-134">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="5a971-135">nome</span><span class="sxs-lookup"><span data-stu-id="5a971-135">name</span></span>     | <span data-ttu-id="5a971-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a971-136">String</span></span> | <span data-ttu-id="5a971-137">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="5a971-137">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="5a971-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a971-138">Response</span></span>

<span data-ttu-id="5a971-139">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a971-139">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a971-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a971-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5a971-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a971-141">Request</span></span>

<span data-ttu-id="5a971-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a971-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5a971-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a971-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```
# <a name="c"></a>[<span data-ttu-id="5a971-144">C#</span><span class="sxs-lookup"><span data-stu-id="5a971-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a971-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a971-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a971-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a971-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a971-147">Java</span><span class="sxs-lookup"><span data-stu-id="5a971-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5a971-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a971-148">Response</span></span>

<span data-ttu-id="5a971-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a971-149">Here is an example of the response.</span></span> <span data-ttu-id="5a971-150">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5a971-150">Note: The response object shown here might be shortened for readability.</span></span>

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
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

