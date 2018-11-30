---
title: Excluir assinatura
description: Exclua uma assinatura.
ms.openlocfilehash: 249393cef11e2768eec0a6435a8485b51cf6921c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007316"
---
# <a name="delete-subscription"></a><span data-ttu-id="8948e-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="8948e-103">Delete subscription</span></span>

<span data-ttu-id="8948e-104">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="8948e-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="8948e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8948e-105">Permissions</span></span>

<span data-ttu-id="8948e-p101">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8948e-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8948e-108">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="8948e-108">Resource type / Item</span></span>        | <span data-ttu-id="8948e-109">Permissão</span><span class="sxs-lookup"><span data-stu-id="8948e-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="8948e-110">Contatos</span><span class="sxs-lookup"><span data-stu-id="8948e-110">Contacts</span></span>                    | <span data-ttu-id="8948e-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8948e-111">Contacts.Read</span></span>       |
| <span data-ttu-id="8948e-112">Conversas</span><span class="sxs-lookup"><span data-stu-id="8948e-112">Conversations</span></span>               | <span data-ttu-id="8948e-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8948e-113">Group.Read.All</span></span>      |
| <span data-ttu-id="8948e-114">Eventos</span><span class="sxs-lookup"><span data-stu-id="8948e-114">Events</span></span>                      | <span data-ttu-id="8948e-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8948e-115">Calendars.Read</span></span>      |
| <span data-ttu-id="8948e-116">Mensagens</span><span class="sxs-lookup"><span data-stu-id="8948e-116">Messages</span></span>                    | <span data-ttu-id="8948e-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8948e-117">Mail.Read</span></span>           |
| <span data-ttu-id="8948e-118">Grupos</span><span class="sxs-lookup"><span data-stu-id="8948e-118">Groups</span></span>                      | <span data-ttu-id="8948e-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8948e-119">Group.Read.All</span></span>      |
| <span data-ttu-id="8948e-120">Usuários</span><span class="sxs-lookup"><span data-stu-id="8948e-120">Users</span></span>                       | <span data-ttu-id="8948e-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8948e-121">User.Read.All</span></span>       |
| <span data-ttu-id="8948e-122">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="8948e-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="8948e-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8948e-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="8948e-124">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="8948e-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="8948e-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8948e-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="8948e-126">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="8948e-126">Security alert</span></span>| <span data-ttu-id="8948e-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8948e-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8948e-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8948e-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8948e-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8948e-129">Request headers</span></span>

| <span data-ttu-id="8948e-130">Nome</span><span class="sxs-lookup"><span data-stu-id="8948e-130">Name</span></span>       | <span data-ttu-id="8948e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8948e-131">Type</span></span> | <span data-ttu-id="8948e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8948e-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8948e-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="8948e-133">Authorization</span></span>  | <span data-ttu-id="8948e-134">string</span><span class="sxs-lookup"><span data-stu-id="8948e-134">string</span></span>  | <span data-ttu-id="8948e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8948e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8948e-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8948e-137">Request body</span></span>

<span data-ttu-id="8948e-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8948e-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8948e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8948e-139">Response</span></span>

<span data-ttu-id="8948e-140">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8948e-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8948e-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8948e-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8948e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8948e-142">Request</span></span>

<span data-ttu-id="8948e-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8948e-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="8948e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8948e-144">Response</span></span>

<span data-ttu-id="8948e-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8948e-145">Here is an example of the response.</span></span>
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
