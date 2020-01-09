---
title: Obter identificadores imutáveis para recursos do Outlook
description: Os identificadores imutáveis permitem que seu aplicativo obtenha uma ID para itens do Outlook que não muda durante a vida útil do item.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: ba38d0aba0063b66c0a51e235c193a57741e9988
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994954"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a><span data-ttu-id="8d092-103">Obter identificadores imutáveis para recursos do Outlook</span><span class="sxs-lookup"><span data-stu-id="8d092-103">Get immutable identifiers for Outlook resources</span></span>

<span data-ttu-id="8d092-104">Itens do Outlook (mensagens, eventos, contatos, tarefas) têm um comportamento interessante que você provavelmente nunca percebeu ou que lhe causou frustração significativa: suas IDs se alteram.</span><span class="sxs-lookup"><span data-stu-id="8d092-104">Outlook items (messages, events, contacts, tasks) have an interesting behavior that you've probably either never noticed or has caused you significant frustration: their IDs change.</span></span> <span data-ttu-id="8d092-105">Isso não acontece com frequência, somente se o item é movido, mas pode causar problemas reais para aplicativos que armazenam IDs offline para uso posterior.</span><span class="sxs-lookup"><span data-stu-id="8d092-105">It doesn't happen often, only if the item is moved, but it can cause real problems for apps that store IDs offline for later use.</span></span> <span data-ttu-id="8d092-106">Identificadores imutáveis permitem que o aplicativo obtenha uma ID que não é alterada durante o tempo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="8d092-106">Immutable identifiers enables your application to obtain an ID that does not change for the lifetime of the item.</span></span>

> [!NOTE]
> <span data-ttu-id="8d092-107">Identificadores imutáveis, como todos os identificadores no Microsoft Graph, diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="8d092-107">Immutable identifiers, like all identifiers in Microsoft Graph, are case-sensitive.</span></span> <span data-ttu-id="8d092-108">Lembre-se disso se você estiver comparando IDs.</span><span class="sxs-lookup"><span data-stu-id="8d092-108">Keep this in mind if you are comparing IDs.</span></span>

## <a name="how-it-works"></a><span data-ttu-id="8d092-109">Como funciona</span><span class="sxs-lookup"><span data-stu-id="8d092-109">How it works</span></span>

<span data-ttu-id="8d092-110">A ID imutável é um recurso opcional do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8d092-110">Immutable ID is an optional feature for Microsoft Graph.</span></span> <span data-ttu-id="8d092-111">Para aceitar, seu aplicativo deve enviar um cabeçalho HTTP adicional em suas solicitações de API:</span><span class="sxs-lookup"><span data-stu-id="8d092-111">To opt in, your application needs to send an additional HTTP header in your API requests:</span></span>

```http
Prefer: IdType="ImmutableId"
```

<span data-ttu-id="8d092-112">Esse cabeçalho só se aplica à solicitação com a qual ele está incluído.</span><span class="sxs-lookup"><span data-stu-id="8d092-112">This header only applies to the request it is included with.</span></span> <span data-ttu-id="8d092-113">Se quiser usar IDs imutáveis, você deverá incluir esse cabeçalho com todas as solicitações de API.</span><span class="sxs-lookup"><span data-stu-id="8d092-113">If you want to always use immutable IDs, you must include this header with every API request.</span></span>

## <a name="lifetime-of-immutable-ids"></a><span data-ttu-id="8d092-114">Tempo de vida das IDs imutáveis</span><span class="sxs-lookup"><span data-stu-id="8d092-114">Lifetime of Immutable IDs</span></span>

<span data-ttu-id="8d092-115">A ID imutável de um item não se alterará, desde que o item permaneça na mesma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8d092-115">An item's immutable ID will not change so long as the item stays in the same mailbox.</span></span> <span data-ttu-id="8d092-116">Isso significa que a ID imutável NÃO será alterada se o item for movido para uma pasta diferente na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8d092-116">That means that immutable ID will NOT change if the item is moved to a different folder in the mailbox.</span></span> <span data-ttu-id="8d092-117">No entanto, a ID imutável será alterada se:</span><span class="sxs-lookup"><span data-stu-id="8d092-117">However, the immutable ID will change if:</span></span>

- <span data-ttu-id="8d092-118">O usuário mover o item para uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="8d092-118">The user moves the item to an archive mailbox.</span></span>
- <span data-ttu-id="8d092-119">O usuário exportar o item (para um PST, como um arquivo MSG, etc.) e importá-lo novamente na sua caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8d092-119">The user exports the item (to a PST, as an MSG file, etc.) and re-imports it into their mailbox.</span></span>
- <span data-ttu-id="8d092-120">O usuário enviar uma mensagem de rascunho.</span><span class="sxs-lookup"><span data-stu-id="8d092-120">The user sends a draft message.</span></span> <span data-ttu-id="8d092-121">A ID imutável da cópia em Itens Enviados não for a mesma ID imutável da mensagem de rascunho.</span><span class="sxs-lookup"><span data-stu-id="8d092-121">The immutable ID of the copy in Sent Items will not be the same immutable ID of the draft message.</span></span>

## <a name="items-that-support-immutable-id"></a><span data-ttu-id="8d092-122">Itens que dão suporte a IDs imutáveis</span><span class="sxs-lookup"><span data-stu-id="8d092-122">Items that support immutable ID</span></span>

<span data-ttu-id="8d092-123">Os seguintes itens dão suporte a IDs imutáveis:</span><span class="sxs-lookup"><span data-stu-id="8d092-123">The following items support immutable IDs:</span></span>

- [<span data-ttu-id="8d092-124">tipo de recurso de mensagem</span><span class="sxs-lookup"><span data-stu-id="8d092-124">message resource type</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="8d092-125">tipo de recurso de anexo</span><span class="sxs-lookup"><span data-stu-id="8d092-125">attachment resource type</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="8d092-126">tipo de recurso de evento</span><span class="sxs-lookup"><span data-stu-id="8d092-126">event resource type</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="8d092-127">tipo de recurso eventMessage</span><span class="sxs-lookup"><span data-stu-id="8d092-127">eventMessage resource type</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="8d092-128">tipo de recurso de contato</span><span class="sxs-lookup"><span data-stu-id="8d092-128">contact resource type</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="8d092-129">tipo de recurso outlookTask</span><span class="sxs-lookup"><span data-stu-id="8d092-129">outlookTask resource type</span></span>](/graph/api/resources/outlooktask)

<span data-ttu-id="8d092-130">Tipos de contêiner (mailFolder, calendário, etc.) não dão suporte a IDs imutáveis, mas suas IDs normais já eram constantes.</span><span class="sxs-lookup"><span data-stu-id="8d092-130">Container types (mailFolder, calendar, etc.) do not support immutable ID, but their regular IDs were already constant.</span></span>

## <a name="immutable-id-with-change-notifications"></a><span data-ttu-id="8d092-131">ID imutável com notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="8d092-131">Immutable ID with change notifications</span></span>

<span data-ttu-id="8d092-132">Você pode solicitar que o Microsoft Graph envie IDs imutáveis em notificações de alteração, incluindo o cabeçalho `Prefer: IdType="ImmutableId"` ao [criar uma assinatura](/graph/api/subscription-post-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="8d092-132">You can request that Microsoft Graph send immutable IDs in change notifications by including the `Prefer: IdType="ImmutableId"` header when [creating a subscription](/graph/api/subscription-post-subscriptions).</span></span> <span data-ttu-id="8d092-133">Assinaturas existentes criadas sem cabeçalho continuarão a usar o formato padrão de ID.</span><span class="sxs-lookup"><span data-stu-id="8d092-133">Existing subscriptions created without the header will continue to use the default ID format.</span></span> <span data-ttu-id="8d092-134">Para fazer com que as assinaturas existentes passem a usar IDs imutáveis, você precisa excluí-las e recriá-las usando o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="8d092-134">In order to switch existing subscriptions to use immutable IDs, you must delete and recreate them using the header.</span></span>

## <a name="immutable-id-with-delta-query"></a><span data-ttu-id="8d092-135">ID imutável com a consulta delta</span><span class="sxs-lookup"><span data-stu-id="8d092-135">Immutable ID with delta query</span></span>

<span data-ttu-id="8d092-136">Ao incluir o cabeçalho `Prefer: IdType="ImmutableId"`, você pode solicitar que o Microsoft Graph retorne IDs imutáveis em [respostas de consulta delta](delta-query-overview.md) para tipos de recursos compatíveis.</span><span class="sxs-lookup"><span data-stu-id="8d092-136">You can request that Microsoft Graph return immutable IDs in [delta query responses](delta-query-overview.md) for supported resource types by including the `Prefer: IdType="ImmutableId"` header.</span></span> <span data-ttu-id="8d092-137">Os valores `nextLink` e `deltaLink` retornados por consultas delta são compatíveis com os dois formatos de ID, então o aplicativo não precisa sincronizar novamente para poder aproveitar o recurso de ID imutável.</span><span class="sxs-lookup"><span data-stu-id="8d092-137">The `nextLink` and `deltaLink` values returned by delta queries are compatible with both ID formats, so your application does not need to re-synchronize to take advantage of immutable ID.</span></span> <span data-ttu-id="8d092-138">Você pode usar o cabeçalho para obter as IDs imutáveis de agora em diante e pode [atualizar o armazenamento do aplicativo](#updating-existing-data) separadamente.</span><span class="sxs-lookup"><span data-stu-id="8d092-138">You can use the header to get immutable IDs going forward, and you can [update your app's storage](#updating-existing-data) separately.</span></span>

## <a name="updating-existing-data"></a><span data-ttu-id="8d092-139">Atualização de dados existentes</span><span class="sxs-lookup"><span data-stu-id="8d092-139">Updating existing data</span></span>

<span data-ttu-id="8d092-140">Se você já tem um banco de dados preenchido com milhares de IDs normais, pode migrar essas IDs para o formato imutável usando a função [translateExchangeIds](/graph/api/user-translateexchangeids).</span><span class="sxs-lookup"><span data-stu-id="8d092-140">If you've already got a database filled with thousands of regular IDs, you can migrate those IDs to immutable format using the [translateExchangeIds](/graph/api/user-translateexchangeids) function.</span></span> <span data-ttu-id="8d092-141">Você pode fornecer uma matriz de até 1.000 IDs para serem convertidas em um formato de destino.</span><span class="sxs-lookup"><span data-stu-id="8d092-141">You can provide an array of up to 1000 IDs to be translated into a target format.</span></span>

> [!NOTE]
> <span data-ttu-id="8d092-142">Você também pode usar `translateExchangeIds` para migrar aplicativos dos Serviços Web do Exchange para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8d092-142">You can also use `translateExchangeIds` to migrate Exchange Web Services applications to Microsoft Graph.</span></span>

### <a name="example"></a><span data-ttu-id="8d092-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d092-143">Example</span></span>

<span data-ttu-id="8d092-144">O exemplo a seguir converte uma ID normal do Graph em uma ID imutável do Graph.</span><span class="sxs-lookup"><span data-stu-id="8d092-144">The following example translates a normal Graph ID to an immutable Graph ID.</span></span>

#### <a name="request"></a><span data-ttu-id="8d092-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d092-145">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/translateExchangeIds

{
  "inputIds" :
  [
    "AQMkAGM2…"
  ],
  "targetIdType" : "restImmutableEntryId",
  "sourceIdType" : "restId"
}
```

#### <a name="response"></a><span data-ttu-id="8d092-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d092-146">Response</span></span>

```http
HTTP 200 OK

{
  "value": [
    {
      "targetId": "AAkALgAA...",
      "sourceId": "AQMkAGM2..."
    }
  ]
}
```
