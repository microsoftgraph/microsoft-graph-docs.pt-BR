---
title: Obter imutáveis identificadores de recursos do Outlook
description: 'Itens do Outlook (mensagens, eventos, contatos, tarefas) têm um comportamento interessante que você provavelmente tiver um nunca percebeu ou causou aborrecimento significativo: altere seus IDs. Isso não acontece com frequência, apenas se o item é movido, mas ele pode causar problemas reais para aplicativos que armazenam IDs offline para uso posterior. Identificadores imutáveis permite que o seu aplicativo obter uma ID que não é alterado para o tempo de vida do item.'
ms.openlocfilehash: a7b188c968ad6e0bf93f92ec99cb473075f29a4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091698"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a><span data-ttu-id="3de85-105">Obter imutáveis identificadores de recursos do Outlook</span><span class="sxs-lookup"><span data-stu-id="3de85-105">Get immutable identifiers for Outlook resources</span></span>

<span data-ttu-id="3de85-106">Itens do Outlook (mensagens, eventos, contatos, tarefas) têm um comportamento interessante que você provavelmente tiver um nunca percebeu ou causou aborrecimento significativo: altere seus IDs.</span><span class="sxs-lookup"><span data-stu-id="3de85-106">Outlook items (messages, events, contacts, tasks) have an interesting behavior that you've probably either never noticed or has caused you significant frustration: their IDs change.</span></span> <span data-ttu-id="3de85-107">Isso não acontece com frequência, apenas se o item é movido, mas ele pode causar problemas reais para aplicativos que armazenam IDs offline para uso posterior.</span><span class="sxs-lookup"><span data-stu-id="3de85-107">It doesn't happen often, only if the item is moved, but it can cause real problems for apps that store IDs offline for later use.</span></span> <span data-ttu-id="3de85-108">Identificadores imutáveis permite que o seu aplicativo obter uma ID que não é alterado para o tempo de vida do item.</span><span class="sxs-lookup"><span data-stu-id="3de85-108">Immutable identifiers enables your application to obtain an ID that does not change for the lifetime of the item.</span></span>

> <span data-ttu-id="3de85-109">**Importante:** Identificadores imutáveis são apenas disponível na versão /beta no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3de85-109">**Important:** Immutable identifiers are only avaiable on the /beta version in Microsoft Graph.</span></span>

## <a name="how-it-works"></a><span data-ttu-id="3de85-110">Como funciona</span><span class="sxs-lookup"><span data-stu-id="3de85-110">How it works</span></span>

<span data-ttu-id="3de85-111">ID imutável é um recurso opcional do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3de85-111">Immutable ID is an optional feature for Microsoft Graph.</span></span> <span data-ttu-id="3de85-112">Para aceitar, seu aplicativo precisa para enviar um cabeçalho HTTP adicional em suas solicitações da API:</span><span class="sxs-lookup"><span data-stu-id="3de85-112">To opt in, your application needs to send an additional HTTP header in your API requests:</span></span>

```http
Prefer: IdType="ImmutableId"
```

<span data-ttu-id="3de85-113">Este cabeçalho se aplica somente a solicitação é incluído com.</span><span class="sxs-lookup"><span data-stu-id="3de85-113">This header only applies to the request it is included with.</span></span> <span data-ttu-id="3de85-114">Se você quiser usar sempre imutáveis IDs, você deve incluir esse cabeçalho com cada solicitação de API.</span><span class="sxs-lookup"><span data-stu-id="3de85-114">If you want to always use immutable IDs, you must include this header with every API request.</span></span>

## <a name="lifetime-of-immutable-ids"></a><span data-ttu-id="3de85-115">Tempo de vida de IDs imutáveis</span><span class="sxs-lookup"><span data-stu-id="3de85-115">Lifetime of Immutable IDs</span></span>

<span data-ttu-id="3de85-116">ID de um item imutáveis não será alterado desde que o item permanece na mesma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="3de85-116">An item's immutable ID will not change so long as the item stays in the same mailbox.</span></span> <span data-ttu-id="3de85-117">Isso significa que imutável ID não será alterada se o item é movido para uma pasta diferente na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="3de85-117">That means that immutable ID will NOT change if the item is moved to a different folder in the mailbox.</span></span> <span data-ttu-id="3de85-118">No entanto, a ID imutável mudarão se:</span><span class="sxs-lookup"><span data-stu-id="3de85-118">However, the immutable ID will change if:</span></span>

- <span data-ttu-id="3de85-119">O usuário move o item para uma caixa de correio de arquivo morto</span><span class="sxs-lookup"><span data-stu-id="3de85-119">The user moves the item to an archive mailbox</span></span>
- <span data-ttu-id="3de85-120">O usuário exporta o item (para um PST, como um arquivo MSG, etc.) e importa-lo novamente em suas caixas de correio</span><span class="sxs-lookup"><span data-stu-id="3de85-120">The user exports the item (to a PST, as an MSG file, etc.) and re-imports it into their mailbox</span></span>

## <a name="items-that-support-immutable-id"></a><span data-ttu-id="3de85-121">Itens que oferecem suporte a ID imutável</span><span class="sxs-lookup"><span data-stu-id="3de85-121">Items that support immutable ID</span></span>

<span data-ttu-id="3de85-122">Os seguintes itens imutáveis IDs de suporte:</span><span class="sxs-lookup"><span data-stu-id="3de85-122">The following items support immutable IDs:</span></span>

- [<span data-ttu-id="3de85-123">tipo de recurso de mensagem</span><span class="sxs-lookup"><span data-stu-id="3de85-123">message resource type</span></span>](/graph/api/resources/message?view=graph-rest-beta)
- [<span data-ttu-id="3de85-124">tipo de recurso attachment</span><span class="sxs-lookup"><span data-stu-id="3de85-124">attachment resource type</span></span>](/graph/api/resources/attachment?view=graph-rest-beta)
- [<span data-ttu-id="3de85-125">tipo de recurso de evento</span><span class="sxs-lookup"><span data-stu-id="3de85-125">event resource type</span></span>](/graph/api/resources/event?view=graph-rest-beta)
- [<span data-ttu-id="3de85-126">Tipo de recurso eventMessage</span><span class="sxs-lookup"><span data-stu-id="3de85-126">eventMessage resource type</span></span>](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [<span data-ttu-id="3de85-127">tipo de recurso contact</span><span class="sxs-lookup"><span data-stu-id="3de85-127">contact resource type</span></span>](/graph/api/resources/contact?view=graph-rest-beta)
- [<span data-ttu-id="3de85-128">tipo de recurso de outlookTask</span><span class="sxs-lookup"><span data-stu-id="3de85-128">outlookTask resource type</span></span>](/graph/api/resources/outlooktask?view=graph-rest-beta)

<span data-ttu-id="3de85-129">Tipos de contêiner (mailFolder, calendário, etc.) não suportam imutável ID, mas seus IDs regulares já foram constantes.</span><span class="sxs-lookup"><span data-stu-id="3de85-129">Container types (mailFolder, calendar, etc.) do not support immutable ID, but their regular IDs were already constant.</span></span>

## <a name="immutable-id-with-change-notifications"></a><span data-ttu-id="3de85-130">ID imutável com notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="3de85-130">Immutable ID with change notifications</span></span>

<span data-ttu-id="3de85-131">Você pode solicitar que o Microsoft Graph enviar notificações de alteração de IDs imutáveis no, incluindo o `Prefer: IdType="ImmutableId"` cabeçalho quando [Criando uma assinatura](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="3de85-131">You can request that Microsoft Graph send immutable IDs in change notifications by including the `Prefer: IdType="ImmutableId"` header when [creating a subscription](/graph/api/subscription-post-subscriptions?view=graph-rest-beta).</span></span> <span data-ttu-id="3de85-132">Inscrições existentes criadas sem o cabeçalho continuará usam o formato de ID de padrão.</span><span class="sxs-lookup"><span data-stu-id="3de85-132">Existing subscriptions created without the header will continue to use the default ID format.</span></span> <span data-ttu-id="3de85-133">Para alternar inscrições existentes para usar IDs imutáveis, você deve excluir e recriá-los usando o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="3de85-133">In order to switch existing subscriptions to use immutable IDs, you must delete and recreate them using the header.</span></span>

## <a name="immutable-id-with-delta-query"></a><span data-ttu-id="3de85-134">ID imutável com consulta delta</span><span class="sxs-lookup"><span data-stu-id="3de85-134">Immutable ID with delta query</span></span>

<span data-ttu-id="3de85-135">Você pode solicitar que o Microsoft Graph retornar IDs imutáveis nas [respostas de consulta delta](delta-query-overview.md) para tipos de recursos com suporte, incluindo o `Prefer: IdType="ImmutableId"` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="3de85-135">You can request that Microsoft Graph return immutable IDs in [delta query responses](delta-query-overview.md) for supported resource types by including the `Prefer: IdType="ImmutableId"` header.</span></span> <span data-ttu-id="3de85-136">O `nextLink` e `deltaLink` valores retornados por consultas delta são compatíveis com ambos os formatos de ID, seu aplicativo precisa sincronizar novamente para se beneficiar dos ID imutável.</span><span class="sxs-lookup"><span data-stu-id="3de85-136">The `nextLink` and `deltaLink` values returned by delta queries are compatible with both ID formats, so your application does not need to re-synchronize to take advantage of immutable ID.</span></span> <span data-ttu-id="3de85-137">Você pode usar o cabeçalho para obter as IDs imutáveis no futuro, e você pode [atualizar o armazenamento do seu aplicativo](#updating-existing-data) separadamente.</span><span class="sxs-lookup"><span data-stu-id="3de85-137">You can use the header to get immutable IDs going forward, and you can [update your app's storage](#updating-existing-data) separately.</span></span>

## <a name="updating-existing-data"></a><span data-ttu-id="3de85-138">Atualizando dados existentes</span><span class="sxs-lookup"><span data-stu-id="3de85-138">Updating existing data</span></span>

<span data-ttu-id="3de85-139">Se você já tem um banco de dados preenchido com milhares de IDs regulares, você pode migrar os IDs de formato imutável usando a função [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="3de85-139">If you've already got a database filled with thousands of regular IDs, you can migrate those IDs to immutable format using the [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) function.</span></span> <span data-ttu-id="3de85-140">Você pode fornecer uma matriz de até 1000 IDs ser traduzidos em um formato de destino.</span><span class="sxs-lookup"><span data-stu-id="3de85-140">You can provide an array of up to 1000 IDs to be translated into a target format.</span></span>

> <span data-ttu-id="3de85-141">**Observação:** Você também pode usar `translateExchangeIds` migrar os aplicativos de serviços Web do Exchange para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3de85-141">**Note:** You can also use `translateExchangeIds` to migrate Exchange Web Services applications to Microsoft Graph.</span></span>

### <a name="example"></a><span data-ttu-id="3de85-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3de85-142">Example</span></span>

<span data-ttu-id="3de85-143">O exemplo a seguir converte uma ID de gráfico normal para uma ID de gráfico imutável.</span><span class="sxs-lookup"><span data-stu-id="3de85-143">The following example translates a normal Graph ID to an immutable Graph ID.</span></span>

#### <a name="request"></a><span data-ttu-id="3de85-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3de85-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds

{
  "inputIds" :
  [
    "AQMkAGM2…"
  ],
  "targetIdType" : "restImmutableEntryId",
  "sourceIdType" : "restId"
}
```

#### <a name="response"></a><span data-ttu-id="3de85-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="3de85-145">Response</span></span>

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