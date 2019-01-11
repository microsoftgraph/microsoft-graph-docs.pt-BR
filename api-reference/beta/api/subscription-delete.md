---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
ms.openlocfilehash: 1e2efb9835e5e625bdac0385b5011cfe5c8c64b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842046"
---
# <a name="delete-subscription"></a><span data-ttu-id="b5e1f-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="b5e1f-103">Delete subscription</span></span>

> <span data-ttu-id="b5e1f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b5e1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5e1f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b5e1f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b5e1f-106">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="b5e1f-106">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5e1f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5e1f-107">Permissions</span></span>

<span data-ttu-id="b5e1f-p102">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5e1f-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5e1f-110">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="b5e1f-110">Resource type / Item</span></span>        | <span data-ttu-id="b5e1f-111">Permissão</span><span class="sxs-lookup"><span data-stu-id="b5e1f-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="b5e1f-112">Contatos</span><span class="sxs-lookup"><span data-stu-id="b5e1f-112">Contacts</span></span>                    | <span data-ttu-id="b5e1f-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b5e1f-113">Contacts.Read</span></span>       |
| <span data-ttu-id="b5e1f-114">Conversas</span><span class="sxs-lookup"><span data-stu-id="b5e1f-114">Conversations</span></span>               | <span data-ttu-id="b5e1f-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5e1f-115">Group.Read.All</span></span>      |
| <span data-ttu-id="b5e1f-116">Eventos</span><span class="sxs-lookup"><span data-stu-id="b5e1f-116">Events</span></span>                      | <span data-ttu-id="b5e1f-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b5e1f-117">Calendars.Read</span></span>      |
| <span data-ttu-id="b5e1f-118">Mensagens</span><span class="sxs-lookup"><span data-stu-id="b5e1f-118">Messages</span></span>                    | <span data-ttu-id="b5e1f-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b5e1f-119">Mail.Read</span></span>           |
| <span data-ttu-id="b5e1f-120">Grupos</span><span class="sxs-lookup"><span data-stu-id="b5e1f-120">Groups</span></span>                      | <span data-ttu-id="b5e1f-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5e1f-121">Group.Read.All</span></span>      |
| <span data-ttu-id="b5e1f-122">Usuários</span><span class="sxs-lookup"><span data-stu-id="b5e1f-122">Users</span></span>                       | <span data-ttu-id="b5e1f-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5e1f-123">User.Read.All</span></span>       |
| <span data-ttu-id="b5e1f-124">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="b5e1f-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="b5e1f-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5e1f-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="b5e1f-126">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="b5e1f-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="b5e1f-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e1f-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="b5e1f-128">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="b5e1f-128">Security alert</span></span>              | <span data-ttu-id="b5e1f-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e1f-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="b5e1f-130">***Observação:*** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="b5e1f-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="b5e1f-131">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b5e1f-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="b5e1f-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e1f-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b5e1f-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5e1f-133">Request headers</span></span>

| <span data-ttu-id="b5e1f-134">Nome</span><span class="sxs-lookup"><span data-stu-id="b5e1f-134">Name</span></span>       | <span data-ttu-id="b5e1f-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5e1f-135">Type</span></span> | <span data-ttu-id="b5e1f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5e1f-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b5e1f-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5e1f-137">Authorization</span></span>  | <span data-ttu-id="b5e1f-138">string</span><span class="sxs-lookup"><span data-stu-id="b5e1f-138">string</span></span>  | <span data-ttu-id="b5e1f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5e1f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5e1f-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5e1f-141">Request body</span></span>

<span data-ttu-id="b5e1f-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5e1f-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5e1f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5e1f-143">Response</span></span>

<span data-ttu-id="b5e1f-144">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b5e1f-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b5e1f-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5e1f-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b5e1f-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5e1f-146">Request</span></span>

<span data-ttu-id="b5e1f-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5e1f-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="b5e1f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5e1f-148">Response</span></span>

<span data-ttu-id="b5e1f-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5e1f-149">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
