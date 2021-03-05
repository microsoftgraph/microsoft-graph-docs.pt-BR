---
title: Obter identificadores imutáveis para recursos do Outlook
description: Os identificadores imutáveis permitem que seu aplicativo obtenha uma ID para itens do Outlook que não muda durante a vida útil do item.
author: abheek-das
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 572804950148e0cf2b5dcbb35842195123698c49
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473655"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a>Obter identificadores imutáveis para recursos do Outlook

Itens do Outlook (mensagens, eventos, contatos, tarefas) têm um comportamento interessante que você provavelmente nunca percebeu ou que lhe causou frustração significativa: suas IDs se alteram. Isso não acontece com frequência, somente se o item é movido, mas pode causar problemas reais para aplicativos que armazenam IDs offline para uso posterior. Identificadores imutáveis permitem que o aplicativo obtenha uma ID que não é alterada durante o tempo de vida do item.

> [!NOTE]
> Identificadores imutáveis, como todos os identificadores no Microsoft Graph, diferenciam maiúsculas de minúsculas. Lembre-se disso se você estiver comparando IDs.

## <a name="how-it-works"></a>Como funciona

A ID imutável é um recurso opcional do Microsoft Graph. Para aceitar, seu aplicativo deve enviar um cabeçalho HTTP adicional em suas solicitações de API:

```http
Prefer: IdType="ImmutableId"
```

Esse cabeçalho só se aplica à solicitação com a qual ele está incluído. Se quiser usar IDs imutáveis, você deverá incluir esse cabeçalho com todas as solicitações de API.

## <a name="lifetime-of-immutable-ids"></a>Tempo de vida das IDs imutáveis

A ID imutável de um item não se alterará, desde que o item permaneça na mesma caixa de correio. Isso significa que a ID imutável NÃO será alterada se o item for movido para uma pasta diferente na caixa de correio. No entanto, a ID imutável será alterada se:

- O usuário mover o item para uma caixa de correio de arquivo morto.
- O usuário exportar o item (para um PST, como um arquivo MSG, etc.) e importá-lo novamente na sua caixa de correio.

## <a name="items-that-support-immutable-id"></a>Itens que dão suporte a IDs imutáveis

Os seguintes itens dão suporte a IDs imutáveis:

- [tipo de recurso de mensagem](/graph/api/resources/message)
- [tipo de recurso de anexo](/graph/api/resources/attachment)
- [tipo de recurso de evento](/graph/api/resources/event)
- [tipo de recurso eventMessage](/graph/api/resources/eventmessage)
- [tipo de recurso de contato](/graph/api/resources/contact)
- [tipo de recurso outlookTask](/graph/api/resources/outlooktask)

Tipos de contêiner (mailFolder, calendário, etc.) não dão suporte a IDs imutáveis, mas suas IDs normais já eram constantes.

## <a name="immutable-id-with-sending-mail"></a>ID imutável com o envio de e-mails

Você pode usar IDs imutáveis para localizar uma mensagem na pasta Itens enviados após ela ter sido enviada, usando as seguintes etapas:

1. [Crie uma mensagem de rascunho](/graph/api/user-post-messages) usando o `Prefer: IdType="ImmutableId"`cabeçalho e salve a `id` propriedade da mensagem na resposta.
1. [Envie a mensagem](/graph/api/message-send) usando a ID da etapa anterior.
1. [Obtenha a mensagem](/graph/api/message-get) usando a ID da primeira etapa. Esta é a cópia em Itens Enviados.

> [!NOTE]
> Obter a mensagem em Itens Enviados pode não ter êxito imediatamente após o envio da mensagem. A cópia da mensagem não será criada até que a mensagem seja enviada com êxito, o que pode levar algum tempo.

## <a name="immutable-id-with-change-notifications"></a>ID imutável com notificações de alteração

Você pode solicitar que o Microsoft Graph envie IDs imutáveis em notificações de alteração, incluindo o cabeçalho `Prefer: IdType="ImmutableId"` ao [criar uma assinatura](/graph/api/subscription-post-subscriptions). Assinaturas existentes criadas sem cabeçalho continuarão a usar o formato padrão de ID. Para fazer com que as assinaturas existentes passem a usar IDs imutáveis, você precisa excluí-las e recriá-las usando o cabeçalho.

## <a name="immutable-id-with-delta-query"></a>ID imutável com a consulta delta

Ao incluir o cabeçalho `Prefer: IdType="ImmutableId"`, você pode solicitar que o Microsoft Graph retorne IDs imutáveis em [respostas de consulta delta](delta-query-overview.md) para tipos de recursos compatíveis. Os valores `nextLink` e `deltaLink` retornados por consultas delta são compatíveis com os dois formatos de ID, então o aplicativo não precisa sincronizar novamente para poder aproveitar o recurso de ID imutável. Você pode usar o cabeçalho para obter as IDs imutáveis de agora em diante e pode [atualizar o armazenamento do aplicativo](#updating-existing-data) separadamente.

## <a name="updating-existing-data"></a>Atualização de dados existentes

Se você já tem um banco de dados preenchido com milhares de IDs normais, pode migrar essas IDs para o formato imutável usando a função [translateExchangeIds](/graph/api/user-translateexchangeids). Você pode fornecer uma matriz de até 1.000 IDs para serem convertidas em um formato de destino.

> [!NOTE]
> Você também pode usar `translateExchangeIds` para migrar aplicativos dos Serviços Web do Exchange para o Microsoft Graph.

### <a name="example"></a>Exemplo

O exemplo a seguir converte uma ID normal do Graph em uma ID imutável do Graph.

#### <a name="request"></a>Solicitação

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

#### <a name="response"></a>Resposta

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
