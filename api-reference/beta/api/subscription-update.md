---
title: Atualizar assinatura
description: Renove uma assinatura ampliando seu tempo de validade.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 19355ff8acbcdade689b140abca63e8d9885e3fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512777"
---
# <a name="update-subscription"></a><span data-ttu-id="ee849-103">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="ee849-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee849-104">Renove uma assinatura ampliando seu tempo de validade.</span><span class="sxs-lookup"><span data-stu-id="ee849-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="ee849-105">Assinaturas expiram após um período de tempo que varia de acordo com o tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="ee849-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="ee849-106">Para evitar notificações de ausentes, um aplicativo deve renovar suas assinaturas bem antes de começar sua data de expiração.</span><span class="sxs-lookup"><span data-stu-id="ee849-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="ee849-107">Consulte [assinatura](../resources/subscription.md) para o comprimento máximo de uma assinatura para cada tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="ee849-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee849-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee849-108">Permissions</span></span>

<span data-ttu-id="ee849-p102">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee849-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee849-111">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="ee849-111">Resource type / Item</span></span>        | <span data-ttu-id="ee849-112">Permissão</span><span class="sxs-lookup"><span data-stu-id="ee849-112">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="ee849-113">Contatos</span><span class="sxs-lookup"><span data-stu-id="ee849-113">Contacts</span></span>                    | <span data-ttu-id="ee849-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ee849-114">Contacts.Read</span></span>       |
| <span data-ttu-id="ee849-115">Conversas</span><span class="sxs-lookup"><span data-stu-id="ee849-115">Conversations</span></span>               | <span data-ttu-id="ee849-116">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee849-116">Group.Read.All</span></span>      |
| <span data-ttu-id="ee849-117">Eventos</span><span class="sxs-lookup"><span data-stu-id="ee849-117">Events</span></span>                      | <span data-ttu-id="ee849-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ee849-118">Calendars.Read</span></span>      |
| <span data-ttu-id="ee849-119">Mensagens</span><span class="sxs-lookup"><span data-stu-id="ee849-119">Messages</span></span>                    | <span data-ttu-id="ee849-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ee849-120">Mail.Read</span></span>           |
| <span data-ttu-id="ee849-121">Grupos</span><span class="sxs-lookup"><span data-stu-id="ee849-121">Groups</span></span>                      | <span data-ttu-id="ee849-122">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee849-122">Group.Read.All</span></span>      |
| <span data-ttu-id="ee849-123">Usuários</span><span class="sxs-lookup"><span data-stu-id="ee849-123">Users</span></span>                       | <span data-ttu-id="ee849-124">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee849-124">User.Read.All</span></span>       |
| <span data-ttu-id="ee849-125">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="ee849-125">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="ee849-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee849-126">Files.ReadWrite</span></span>     |
| <span data-ttu-id="ee849-127">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="ee849-127">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="ee849-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee849-128">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="ee849-129">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="ee849-129">Security alert</span></span>               | <span data-ttu-id="ee849-130">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee849-130">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="ee849-131">***Observação:*** O ponto de extremidade /beta permite que as permissões de aplicativo para a maioria dos recursos.</span><span class="sxs-lookup"><span data-stu-id="ee849-131">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="ee849-132">Não há suporte para conversas em itens de raiz uma unidade OneDrive e de grupo com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ee849-132">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="ee849-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee849-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ee849-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee849-134">Request headers</span></span>

| <span data-ttu-id="ee849-135">Nome</span><span class="sxs-lookup"><span data-stu-id="ee849-135">Name</span></span>       | <span data-ttu-id="ee849-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee849-136">Type</span></span> | <span data-ttu-id="ee849-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee849-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ee849-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee849-138">Authorization</span></span>  | <span data-ttu-id="ee849-139">string</span><span class="sxs-lookup"><span data-stu-id="ee849-139">string</span></span>  | <span data-ttu-id="ee849-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee849-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ee849-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee849-142">Response</span></span>

<span data-ttu-id="ee849-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee849-143">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee849-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee849-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee849-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee849-145">Request</span></span>

<span data-ttu-id="ee849-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee849-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="ee849-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee849-147">Response</span></span>

<span data-ttu-id="ee849-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee849-148">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
