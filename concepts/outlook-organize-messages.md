---
title: Organize mensagens do Outlook usando a API de email do Outlook
description: Organize as suas mensagens do Outlook do jeito que você gosta. Filtre, pesquise ou classifique mensagens de forma conveniente em toda a sua caixa de correio ou em pastas específicas.
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: e2c098234e1ea37e98e22153e56b6d88783e9f0c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444317"
---
# <a name="organize-outlook-messages"></a>Organizar mensagens do Outlook

O Outlook permite que os clientes organizem suas mensagens da maneira que quiserem, seja deixando todas na mesma pasta da Caixa de Entrada ou organizando-as em uma estrutura de pastas em forma de árvore na Caixa de Entrada para atender a necessidades específicas. Você pode convenientemente [filtrar, pesquisar ou classificar](query-parameters.md) mensagens na caixa de correio inteira do usuário ou em pastas específicas.

## <a name="access-mail-folders"></a>Acessar pastas de email

De forma programática, as pastas de mensagens são representadas pelo recurso [mailFolder](/graph/api/resources/mailfolder) e a Caixa de Entrada é uma das pastas na raiz da estrutura de pastas.

Cada **mailFolder** identificado por sua ID de pasta e tem uma propriedade **displayName** gravável. O Outlook cria algumas outras pastas para usuários por padrão. Você pode fazer referência a essas pastas padrão usando suas IDs de pasta ou seus nomes conhecidos. Confira uma lista de nomes de pasta comuns disponíveis em [Tipo de recurso mailFolder](/graph/api/resources/mailfolder).

No caso de uma pasta personalizada, não padrão, se você souber o caminho da pasta, poderá acessar a pasta primeiro usando o atalho `/users/{id}/mailfolders` para chegar ao nível raiz e obter todas as pastas de nível superior:

```http
GET https://graph.microsoft.com/v1.0/users/{id}/mailFolders
```

Em seguida, especifique a ID da pasta apropriada (`{folder_id}`) à medida que você navega em cada nível da árvore de pastas:

```http
GET https://graph.microsoft.com/v1.0/users/{id}/mailFolders/{folder_id}/childfolders
```

Repita a operação até chegar finalmente à pasta personalizada na árvore.

## <a name="create-and-organize-the-folder-tree"></a>Criar e organizar a árvore de pastas

Você pode [criar pastas de email na Caixa de Entrada](/graph/api/user-post-mailfolders) ou como [pastas filhas de outras pastas](/graph/api/mailfolder-post-childfolders). Ao criar, [copiar](/graph/api/mailfolder-copy) ou [mover](/graph/api/mailfolder-move) uma pasta e seu conteúdo, o Outlook atualizará as propriedades somente leitura **parentFolderId** e **childFolderCount** das pastas envolvidas. Quando o conteúdo de uma pasta for copiado ou movido para outra pasta, por padrão, as IDs de entrada individuais do conteúdo também serão alteradas.

No nível do conteúdo, **totalItemCount** e **unreadItemCount** respectivamente informam o número de itens e o número de itens não lidos em uma pasta de email.
No nível das pastas filho, você pode [listar as pastas filho](/graph/api/user-list-mailfolders) na Caixa de Entrada ou em qualquer outra pasta.
A propriedade **childFolderCount** representa o número de pastas filho imediatas.

Lembre-se de que as pastas de email do Outlook podem conter mensagens e itens que não são de mensagens, como eventos e contatos. Em geral, as pastas do Outlook podem conter itens heterogêneos.

## <a name="use-rules-to-automate-copying-or-moving-messages"></a>Use regras para automatizar a cópia ou a transferência de mensagens

O Outlook permite que os clientes definam regras para automatizar ações específicas em mensagens recebidas quando algumas condições pré-determinadas forem atendidas. Você pode [criar uma regra](/graph/api/mailfolder-post-messagerules) para a Caixa de Entrada como uma [messageRule](/graph/api/resources/messagerule) para copiar ou mover uma mensagem para uma pasta específica em determinadas condições.
As condições são [messageRulePredicates](/graph/api/resources/messagerulepredicates). Elas podem incluir o assunto ou o corpo da mensagem contendo determinado texto, a mensagem enviada de determinados endereços de email ou a mensagem marcada como importante e assim por diante.

## <a name="direct-only-the-messages-you-care-about-to-the-focused-inbox"></a>Direcione apenas as mensagens de seu interesse para a Caixa de Entrada Destaques

A Caixa de Entrada Destaques permite que os clientes treinem o Outlook para mostrar apenas as mensagens recebidas dos remetentes que te interessam na guia **Destaques** e o restante na guia **Outros**. Inicialmente, o sistema de classificação do Outlook organizará as mensagens da Caixa de Entrada de maneira padrão. Ao longo do tempo, você poderá corrigir e treinar o sistema por meio da interface do usuário ou programaticamente. Quanto mais você usar a Caixa de Entrada Destaques, melhor o sistema de classificação conseguirá deduzir o que você deseja ver na mensagem de entrada na guia **Destaques**.

Programaticamente, você poderá atualizar a propriedade **inferenceClassification** de uma [mensagem](/graph/api/resources/message) para indicar se deseja ver a mensagem na guia **Destaques** ou **Outros**. Essa é uma designação única para uma mensagem específica. Se, por outro lado, você quiser ver as mensagens de um remetente específico sempre na guia **Destaques** ou **Outros**, [defina uma instrução](/graph/api/inferenceclassification-post-overrides) para o Outlook. Cada instrução é uma instância [inferenceClassificationOverride](/graph/api/resources/inferenceclassificationoverride) que especifica o nome do remetente e sua designação para que as mensagens desse remetente sejam sempre `focused` ou `other`. As instruções de cada usuário para a Caixa de Entrada Destaques do usuário são armazenadas como uma coleção de instâncias [inferenceClassificationOverride](/graph/api/resources/inferenceclassificationoverride) no objeto [user](/graph/api/resources/user).

## <a name="keep-messages-and-mail-folders-up-to-date-in-apps"></a>Mantenha mensagens e pastas de e-mail atualizadas nos aplicativos

Os aplicativos geralmente precisam sincronizar e manter atualizados os dados de email de um usuário na loja local do aplicativo. O Microsoft Graph permite que você se inscreva nas notificações de alterações para receber notificações quando os dados forem alterados e consultar alterações reais assim que elas ocorrerem.

As notificações serão enviadas por [webhooks](/graph/api/resources/webhooks) de forma assíncrona quando as alterações ocorrerem, evitando que os aplicativos tenham que pesquisar com frequência. Você pode [inscrever-se nas notificações de alteração](/graph/api/subscription-post-subscriptions) para informar-se sobre novidades, atualizações ou exclusões de dados de email do usuário. Por exemplo, você pode criar uma inscrição para mensagens em uma pasta específica (por exemplo, `/me/mailFolders('{folderId'}')`) ou no nível raiz (por exemplo, `/me/messages`). A assinatura especifica uma **notificationUrl** onde o Microsoft Graph notificará o aplicativo quando os tipos solicitados de alterações ocorrerem.

Para sincronizar inicialmente a caixa de correio de um usuário, primeiro, [realize uma consulta delta das pastas de email iniciando no nível raiz](/graph/api/mailfolder-delta) para sincronizar todas as pastas de email, seguido por uma [consulta delta das mensagens em cada pasta](/graph/api/message-delta) para sincronizar mensagens individuais.

Para localizar as entidades exatas que foram alteradas sem ler todo o recurso a cada notificação, você pode usar a [consulta delta](delta-query-overview.md) para controlar essas alterações importantes e sincronizar sua loja local com essas alterações. Você pode [controlar alterações em mensagens em uma pasta específica](delta-query-messages.md). Também é possível controlar alterações em pastas de email no nível raiz (ou seja, `/me/mailfolders`).

## <a name="next-steps"></a>Próximas etapas

- [Por que integrar-se com o email do Outlook](outlook-mail-concept-overview.md)
- [Usar a API de email](/graph/api/resources/mail-api-overview) e seus [casos de uso](/graph/api/resources/mail-api-overview#common-use-cases) no Microsoft Graph versão 1.0.
