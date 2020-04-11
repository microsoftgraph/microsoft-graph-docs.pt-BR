---
title: Atualizar calendarpermission
description: Atualize as propriedades do objeto calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b990b038960a97eb8ba8e86d6a338cebe4339fbb
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227749"
---
# <a name="update-calendarpermission"></a><span data-ttu-id="0d605-103">Atualizar calendarPermission</span><span class="sxs-lookup"><span data-stu-id="0d605-103">Update calendarPermission</span></span>

<span data-ttu-id="0d605-104">Atualize as permissões atribuídas a um compartilhamento ou delegado existente, através do objeto [calendarPermission](../resources/calendarpermission.md) correspondente para um calendário.</span><span class="sxs-lookup"><span data-stu-id="0d605-104">Update the permissions assigned to an existing sharee or delegate, through the corresponding [calendarPermission](../resources/calendarpermission.md) object for a calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d605-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d605-105">Permissions</span></span>

<span data-ttu-id="0d605-106">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="0d605-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="0d605-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d605-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d605-108">Calendário</span><span class="sxs-lookup"><span data-stu-id="0d605-108">Calendar</span></span> | <span data-ttu-id="0d605-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d605-109">Delegated (work or school account)</span></span> | <span data-ttu-id="0d605-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d605-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d605-111">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d605-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="0d605-112">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="0d605-112">user calendar</span></span> | <span data-ttu-id="0d605-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d605-113">Calendars.ReadWrite</span></span> | <span data-ttu-id="0d605-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d605-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="0d605-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d605-115">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="0d605-116">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="0d605-116">group calendar</span></span> | <span data-ttu-id="0d605-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d605-117">Group.ReadWrite.All</span></span> | <span data-ttu-id="0d605-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d605-118">Not supported.</span></span> | <span data-ttu-id="0d605-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d605-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d605-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d605-120">HTTP request</span></span>

<span data-ttu-id="0d605-121">Atualizar as permissões especificadas do calendário de um usuário:</span><span class="sxs-lookup"><span data-stu-id="0d605-121">Update the specified permissions of a user's calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="0d605-122">Atualizar as permissões especificadas de um calendário de Grupo:</span><span class="sxs-lookup"><span data-stu-id="0d605-122">Update the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="0d605-123">Atualize as permissões especificadas do calendário do usuário que contém o evento identificado:</span><span class="sxs-lookup"><span data-stu-id="0d605-123">Update the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0d605-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d605-124">Request headers</span></span>

| <span data-ttu-id="0d605-125">Nome</span><span class="sxs-lookup"><span data-stu-id="0d605-125">Name</span></span>       | <span data-ttu-id="0d605-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d605-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0d605-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d605-127">Authorization</span></span> | <span data-ttu-id="0d605-128">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="0d605-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d605-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d605-129">Request body</span></span>

<span data-ttu-id="0d605-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="0d605-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0d605-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="0d605-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0d605-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="0d605-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0d605-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d605-133">Property</span></span>     | <span data-ttu-id="0d605-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d605-134">Type</span></span>        | <span data-ttu-id="0d605-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d605-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d605-136">role</span><span class="sxs-lookup"><span data-stu-id="0d605-136">role</span></span>|[<span data-ttu-id="0d605-137">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="0d605-137">calendarRoleType</span></span>](../resources/calendarpermission.md#calendarroletype-values)| <span data-ttu-id="0d605-138">O nível de permissão a ser alterado para o compartilhamento ou representante do calendário.</span><span class="sxs-lookup"><span data-stu-id="0d605-138">The permission level to change to for the calendar sharee or delegate.</span></span> |

## <a name="response"></a><span data-ttu-id="0d605-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d605-139">Response</span></span>

<span data-ttu-id="0d605-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [calendarPermission](../resources/calendarpermission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d605-140">If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d605-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d605-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d605-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d605-142">Request</span></span>

<span data-ttu-id="0d605-143">O exemplo a seguir altera o nível de permissão de Sharee, Adele, `write`para.</span><span class="sxs-lookup"><span data-stu-id="0d605-143">The following example changes the permission level of the sharee, Adele, to `write`.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["RGVmYXVsdA=="],
  "name": "update_calendarpermission"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/RGVmYXVsdA==
Content-type: application/json

{
  "role": "write"
}
```

### <a name="response"></a><span data-ttu-id="0d605-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d605-144">Response</span></span>

<span data-ttu-id="0d605-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d605-145">The following is an example of the response.</span></span>

> <span data-ttu-id="0d605-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d605-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "update_calendarpermission",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "L289RXhlbGVW",
    "isRemovable": true,
    "isInsideOrganization": true,
    "role": "write",
    "allowedRoles": [
        "freeBusyRead",
        "limitedRead",
        "read",
        "write"
    ],
    "emailAddress": {
        "name": "Adele Vance",
        "address": "AdeleV@contoso.OnMicrosoft.com"
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update calendarpermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
