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
# <a name="get-immutable-identifiers-for-outlook-resources"></a>Obter imutáveis identificadores de recursos do Outlook

Itens do Outlook (mensagens, eventos, contatos, tarefas) têm um comportamento interessante que você provavelmente tiver um nunca percebeu ou causou aborrecimento significativo: altere seus IDs. Isso não acontece com frequência, apenas se o item é movido, mas ele pode causar problemas reais para aplicativos que armazenam IDs offline para uso posterior. Identificadores imutáveis permite que o seu aplicativo obter uma ID que não é alterado para o tempo de vida do item.

> **Importante:** Identificadores imutáveis são apenas disponível na versão /beta no Microsoft Graph.

## <a name="how-it-works"></a>Como funciona

ID imutável é um recurso opcional do Microsoft Graph. Para aceitar, seu aplicativo precisa para enviar um cabeçalho HTTP adicional em suas solicitações da API:

```http
Prefer: IdType="ImmutableId"
```

Este cabeçalho se aplica somente a solicitação é incluído com. Se você quiser usar sempre imutáveis IDs, você deve incluir esse cabeçalho com cada solicitação de API.

## <a name="lifetime-of-immutable-ids"></a>Tempo de vida de IDs imutáveis

ID de um item imutáveis não será alterado desde que o item permanece na mesma caixa de correio. Isso significa que imutável ID não será alterada se o item é movido para uma pasta diferente na caixa de correio. No entanto, a ID imutável mudarão se:

- O usuário move o item para uma caixa de correio de arquivo morto
- O usuário exporta o item (para um PST, como um arquivo MSG, etc.) e importa-lo novamente em suas caixas de correio

## <a name="items-that-support-immutable-id"></a>Itens que oferecem suporte a ID imutável

Os seguintes itens imutáveis IDs de suporte:

- [tipo de recurso de mensagem](/graph/api/resources/message?view=graph-rest-beta)
- [tipo de recurso attachment](/graph/api/resources/attachment?view=graph-rest-beta)
- [tipo de recurso de evento](/graph/api/resources/event?view=graph-rest-beta)
- [Tipo de recurso eventMessage](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [tipo de recurso contact](/graph/api/resources/contact?view=graph-rest-beta)
- [tipo de recurso de outlookTask](/graph/api/resources/outlooktask?view=graph-rest-beta)

Tipos de contêiner (mailFolder, calendário, etc.) não suportam imutável ID, mas seus IDs regulares já foram constantes.

## <a name="immutable-id-with-change-notifications"></a>ID imutável com notificações de alteração

Você pode solicitar que o Microsoft Graph enviar notificações de alteração de IDs imutáveis no, incluindo o `Prefer: IdType="ImmutableId"` cabeçalho quando [Criando uma assinatura](/graph/api/subscription-post-subscriptions?view=graph-rest-beta). Inscrições existentes criadas sem o cabeçalho continuará usam o formato de ID de padrão. Para alternar inscrições existentes para usar IDs imutáveis, você deve excluir e recriá-los usando o cabeçalho.

## <a name="immutable-id-with-delta-query"></a>ID imutável com consulta delta

Você pode solicitar que o Microsoft Graph retornar IDs imutáveis nas [respostas de consulta delta](delta-query-overview.md) para tipos de recursos com suporte, incluindo o `Prefer: IdType="ImmutableId"` cabeçalho. O `nextLink` e `deltaLink` valores retornados por consultas delta são compatíveis com ambos os formatos de ID, seu aplicativo precisa sincronizar novamente para se beneficiar dos ID imutável. Você pode usar o cabeçalho para obter as IDs imutáveis no futuro, e você pode [atualizar o armazenamento do seu aplicativo](#updating-existing-data) separadamente.

## <a name="updating-existing-data"></a>Atualizando dados existentes

Se você já tem um banco de dados preenchido com milhares de IDs regulares, você pode migrar os IDs de formato imutável usando a função [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) . Você pode fornecer uma matriz de até 1000 IDs ser traduzidos em um formato de destino.

> **Observação:** Você também pode usar `translateExchangeIds` migrar os aplicativos de serviços Web do Exchange para o Microsoft Graph.

### <a name="example"></a>Exemplo

O exemplo a seguir converte uma ID de gráfico normal para uma ID de gráfico imutável.

#### <a name="request"></a>Solicitação

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