---
title: Atualizar calendargroup
description: Atualizar as propriedades do objeto calendargroup.
author: angelgolfer-ms
ms.openlocfilehash: e0e2cbc9ef2f86298d320285163e2e7378a8f3ec
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336699"
---
# <a name="update-calendargroup"></a><span data-ttu-id="e62ea-103">Atualizar calendargroup</span><span class="sxs-lookup"><span data-stu-id="e62ea-103">Update calendargroup</span></span>

> <span data-ttu-id="e62ea-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e62ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e62ea-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e62ea-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e62ea-106">Atualizar as propriedades do objeto calendargroup.</span><span class="sxs-lookup"><span data-stu-id="e62ea-106">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e62ea-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e62ea-107">Permissions</span></span>

<span data-ttu-id="e62ea-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e62ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e62ea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e62ea-110">Permission type</span></span>                        | <span data-ttu-id="e62ea-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e62ea-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e62ea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e62ea-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e62ea-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e62ea-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="e62ea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e62ea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e62ea-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e62ea-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="e62ea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e62ea-116">Application</span></span>                            | <span data-ttu-id="e62ea-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e62ea-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e62ea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e62ea-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="e62ea-119">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e62ea-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e62ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e62ea-120">Request headers</span></span>

| <span data-ttu-id="e62ea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e62ea-121">Header</span></span>        | <span data-ttu-id="e62ea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e62ea-122">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="e62ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e62ea-123">Authorization</span></span> | <span data-ttu-id="e62ea-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e62ea-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e62ea-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e62ea-126">Content-Type</span></span>  | <span data-ttu-id="e62ea-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e62ea-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e62ea-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e62ea-129">Request body</span></span>

<span data-ttu-id="e62ea-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e62ea-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e62ea-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e62ea-133">Property</span></span> | <span data-ttu-id="e62ea-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="e62ea-134">Type</span></span>   | <span data-ttu-id="e62ea-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e62ea-135">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="e62ea-136">name</span><span class="sxs-lookup"><span data-stu-id="e62ea-136">name</span></span>     | <span data-ttu-id="e62ea-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e62ea-137">String</span></span> | <span data-ttu-id="e62ea-138">O nome do grupo.</span><span class="sxs-lookup"><span data-stu-id="e62ea-138">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="e62ea-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e62ea-139">Response</span></span>

<span data-ttu-id="e62ea-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e62ea-140">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e62ea-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e62ea-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e62ea-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e62ea-142">Request</span></span>

<span data-ttu-id="e62ea-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e62ea-143">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="e62ea-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e62ea-144">Response</span></span>

<span data-ttu-id="e62ea-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e62ea-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
