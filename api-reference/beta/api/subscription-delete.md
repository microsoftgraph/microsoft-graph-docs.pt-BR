---
title: Excluir assinatura
description: Exclua uma assinatura.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9ca4c772cb6d7de088550a16262275b4c43fb9c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509459"
---
# <a name="delete-subscription"></a><span data-ttu-id="e35c2-103">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="e35c2-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e35c2-104">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="e35c2-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="e35c2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e35c2-105">Permissions</span></span>

<span data-ttu-id="e35c2-p101">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e35c2-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e35c2-108">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="e35c2-108">Resource type / Item</span></span>        | <span data-ttu-id="e35c2-109">Permissão</span><span class="sxs-lookup"><span data-stu-id="e35c2-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="e35c2-110">Contatos</span><span class="sxs-lookup"><span data-stu-id="e35c2-110">Contacts</span></span>                    | <span data-ttu-id="e35c2-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="e35c2-111">Contacts.Read</span></span>       |
| <span data-ttu-id="e35c2-112">Conversas</span><span class="sxs-lookup"><span data-stu-id="e35c2-112">Conversations</span></span>               | <span data-ttu-id="e35c2-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e35c2-113">Group.Read.All</span></span>      |
| <span data-ttu-id="e35c2-114">Eventos</span><span class="sxs-lookup"><span data-stu-id="e35c2-114">Events</span></span>                      | <span data-ttu-id="e35c2-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e35c2-115">Calendars.Read</span></span>      |
| <span data-ttu-id="e35c2-116">Mensagens</span><span class="sxs-lookup"><span data-stu-id="e35c2-116">Messages</span></span>                    | <span data-ttu-id="e35c2-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e35c2-117">Mail.Read</span></span>           |
| <span data-ttu-id="e35c2-118">Grupos</span><span class="sxs-lookup"><span data-stu-id="e35c2-118">Groups</span></span>                      | <span data-ttu-id="e35c2-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e35c2-119">Group.Read.All</span></span>      |
| <span data-ttu-id="e35c2-120">Usuários</span><span class="sxs-lookup"><span data-stu-id="e35c2-120">Users</span></span>                       | <span data-ttu-id="e35c2-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="e35c2-121">User.Read.All</span></span>       |
| <span data-ttu-id="e35c2-122">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="e35c2-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="e35c2-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e35c2-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="e35c2-124">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="e35c2-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="e35c2-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e35c2-125">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="e35c2-126">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="e35c2-126">Security alert</span></span>              | <span data-ttu-id="e35c2-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e35c2-127">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="e35c2-128">***Observação:*** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="e35c2-128">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="e35c2-129">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e35c2-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="e35c2-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e35c2-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e35c2-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e35c2-131">Request headers</span></span>

| <span data-ttu-id="e35c2-132">Nome</span><span class="sxs-lookup"><span data-stu-id="e35c2-132">Name</span></span>       | <span data-ttu-id="e35c2-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e35c2-133">Type</span></span> | <span data-ttu-id="e35c2-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e35c2-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e35c2-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="e35c2-135">Authorization</span></span>  | <span data-ttu-id="e35c2-136">string</span><span class="sxs-lookup"><span data-stu-id="e35c2-136">string</span></span>  | <span data-ttu-id="e35c2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e35c2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e35c2-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e35c2-139">Request body</span></span>

<span data-ttu-id="e35c2-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e35c2-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e35c2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e35c2-141">Response</span></span>

<span data-ttu-id="e35c2-142">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e35c2-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e35c2-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e35c2-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e35c2-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e35c2-144">Request</span></span>

<span data-ttu-id="e35c2-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e35c2-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="e35c2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e35c2-146">Response</span></span>

<span data-ttu-id="e35c2-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e35c2-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
