---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 79ffce638036414469953d6d729229e00cb1662f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945871"
---
# <a name="delete-subscription"></a><span data-ttu-id="07d74-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="07d74-103">Delete subscription</span></span>

> <span data-ttu-id="07d74-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="07d74-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07d74-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="07d74-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07d74-106">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="07d74-106">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="07d74-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="07d74-107">Permissions</span></span>

<span data-ttu-id="07d74-p102">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07d74-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07d74-110">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="07d74-110">Resource type / Item</span></span>        | <span data-ttu-id="07d74-111">Permissão</span><span class="sxs-lookup"><span data-stu-id="07d74-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="07d74-112">Contatos</span><span class="sxs-lookup"><span data-stu-id="07d74-112">Contacts</span></span>                    | <span data-ttu-id="07d74-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="07d74-113">Contacts.Read</span></span>       |
| <span data-ttu-id="07d74-114">Conversas</span><span class="sxs-lookup"><span data-stu-id="07d74-114">Conversations</span></span>               | <span data-ttu-id="07d74-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="07d74-115">Group.Read.All</span></span>      |
| <span data-ttu-id="07d74-116">Eventos</span><span class="sxs-lookup"><span data-stu-id="07d74-116">Events</span></span>                      | <span data-ttu-id="07d74-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="07d74-117">Calendars.Read</span></span>      |
| <span data-ttu-id="07d74-118">Mensagens</span><span class="sxs-lookup"><span data-stu-id="07d74-118">Messages</span></span>                    | <span data-ttu-id="07d74-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07d74-119">Mail.Read</span></span>           |
| <span data-ttu-id="07d74-120">Grupos</span><span class="sxs-lookup"><span data-stu-id="07d74-120">Groups</span></span>                      | <span data-ttu-id="07d74-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="07d74-121">Group.Read.All</span></span>      |
| <span data-ttu-id="07d74-122">Usuários</span><span class="sxs-lookup"><span data-stu-id="07d74-122">Users</span></span>                       | <span data-ttu-id="07d74-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="07d74-123">User.Read.All</span></span>       |
| <span data-ttu-id="07d74-124">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="07d74-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="07d74-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="07d74-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="07d74-126">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="07d74-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="07d74-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d74-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="07d74-128">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="07d74-128">Security alert</span></span>              | <span data-ttu-id="07d74-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d74-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="07d74-130">***Observação:*** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="07d74-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="07d74-131">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="07d74-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="07d74-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07d74-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="07d74-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07d74-133">Request headers</span></span>

| <span data-ttu-id="07d74-134">Nome</span><span class="sxs-lookup"><span data-stu-id="07d74-134">Name</span></span>       | <span data-ttu-id="07d74-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="07d74-135">Type</span></span> | <span data-ttu-id="07d74-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="07d74-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="07d74-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="07d74-137">Authorization</span></span>  | <span data-ttu-id="07d74-138">string</span><span class="sxs-lookup"><span data-stu-id="07d74-138">string</span></span>  | <span data-ttu-id="07d74-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07d74-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07d74-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07d74-141">Request body</span></span>

<span data-ttu-id="07d74-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07d74-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07d74-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="07d74-143">Response</span></span>

<span data-ttu-id="07d74-144">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="07d74-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07d74-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07d74-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="07d74-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07d74-146">Request</span></span>

<span data-ttu-id="07d74-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07d74-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="07d74-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="07d74-148">Response</span></span>

<span data-ttu-id="07d74-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07d74-149">Here is an example of the response.</span></span>
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
