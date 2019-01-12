---
title: Atualizar calendargroup
description: Atualizar as propriedades do objeto calendargroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f488594778c1e80e725cb2587bf5d0c41cb570e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961299"
---
# <a name="update-calendargroup"></a><span data-ttu-id="dfb32-103">Atualizar calendargroup</span><span class="sxs-lookup"><span data-stu-id="dfb32-103">Update calendargroup</span></span>

> <span data-ttu-id="dfb32-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dfb32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfb32-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dfb32-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dfb32-106">Atualizar as propriedades do objeto calendargroup.</span><span class="sxs-lookup"><span data-stu-id="dfb32-106">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfb32-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfb32-107">Permissions</span></span>

<span data-ttu-id="dfb32-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfb32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfb32-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfb32-110">Permission type</span></span>                        | <span data-ttu-id="dfb32-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfb32-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="dfb32-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfb32-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfb32-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfb32-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="dfb32-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfb32-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfb32-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfb32-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="dfb32-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfb32-116">Application</span></span>                            | <span data-ttu-id="dfb32-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfb32-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dfb32-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfb32-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="dfb32-119">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="dfb32-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dfb32-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb32-120">Request headers</span></span>

| <span data-ttu-id="dfb32-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dfb32-121">Header</span></span>        | <span data-ttu-id="dfb32-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dfb32-122">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="dfb32-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfb32-123">Authorization</span></span> | <span data-ttu-id="dfb32-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfb32-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="dfb32-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dfb32-126">Content-Type</span></span>  | <span data-ttu-id="dfb32-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfb32-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfb32-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb32-129">Request body</span></span>

<span data-ttu-id="dfb32-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="dfb32-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dfb32-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dfb32-133">Property</span></span> | <span data-ttu-id="dfb32-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfb32-134">Type</span></span>   | <span data-ttu-id="dfb32-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfb32-135">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="dfb32-136">name</span><span class="sxs-lookup"><span data-stu-id="dfb32-136">name</span></span>     | <span data-ttu-id="dfb32-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dfb32-137">String</span></span> | <span data-ttu-id="dfb32-138">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="dfb32-138">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="dfb32-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfb32-139">Response</span></span>

<span data-ttu-id="dfb32-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfb32-140">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfb32-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfb32-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dfb32-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb32-142">Request</span></span>

<span data-ttu-id="dfb32-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfb32-143">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="dfb32-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfb32-144">Response</span></span>

<span data-ttu-id="dfb32-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfb32-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
