---
title: Atualizar calendargroup
description: Atualiza as propriedades do objeto calendargroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e093ddd962b1fa0397159c47bdc5388184a8ba3c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583729"
---
# <a name="update-calendargroup"></a><span data-ttu-id="2f85d-103">Atualizar calendargroup</span><span class="sxs-lookup"><span data-stu-id="2f85d-103">Update calendargroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f85d-104">Atualiza as propriedades do objeto calendargroup.</span><span class="sxs-lookup"><span data-stu-id="2f85d-104">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f85d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f85d-105">Permissions</span></span>

<span data-ttu-id="2f85d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f85d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f85d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f85d-108">Permission type</span></span>                        | <span data-ttu-id="2f85d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f85d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2f85d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f85d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f85d-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f85d-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="2f85d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f85d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f85d-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f85d-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="2f85d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f85d-114">Application</span></span>                            | <span data-ttu-id="2f85d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f85d-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2f85d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f85d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="2f85d-117">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2f85d-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2f85d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f85d-118">Request headers</span></span>

| <span data-ttu-id="2f85d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f85d-119">Header</span></span>        | <span data-ttu-id="2f85d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2f85d-120">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="2f85d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f85d-121">Authorization</span></span> | <span data-ttu-id="2f85d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f85d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2f85d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f85d-124">Content-Type</span></span>  | <span data-ttu-id="2f85d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f85d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f85d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f85d-127">Request body</span></span>

<span data-ttu-id="2f85d-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2f85d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2f85d-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f85d-131">Property</span></span> | <span data-ttu-id="2f85d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f85d-132">Type</span></span>   | <span data-ttu-id="2f85d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f85d-133">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="2f85d-134">name</span><span class="sxs-lookup"><span data-stu-id="2f85d-134">name</span></span>     | <span data-ttu-id="2f85d-135">String</span><span class="sxs-lookup"><span data-stu-id="2f85d-135">String</span></span> | <span data-ttu-id="2f85d-136">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="2f85d-136">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="2f85d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f85d-137">Response</span></span>

<span data-ttu-id="2f85d-138">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f85d-138">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f85d-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f85d-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2f85d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f85d-140">Request</span></span>

<span data-ttu-id="2f85d-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f85d-141">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="2f85d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f85d-142">Response</span></span>

<span data-ttu-id="2f85d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f85d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
