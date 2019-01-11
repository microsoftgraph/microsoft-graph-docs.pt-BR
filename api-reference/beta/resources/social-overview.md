---
title: Usar a API do Microsoft Graph para integrar inteligência social em um aplicativo
description: O Microsoft Graph suporta gestos sociais em um contexto do usuário social e fornece acesso às pessoas útil e dados sociais.
localization_priority: Priority
ms.openlocfilehash: b3b71cf1bad0d860978c75c88f0b77a32eab1a0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862486"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a>Usar a API do Microsoft Graph para integrar inteligência social em um aplicativo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O Microsoft Graph suporta gestos sociais em um contexto do usuário social e fornece acesso às pessoas útil e dados sociais.

## <a name="aggregate-and-extract-specific-information-about-people"></a>Agregadas e extrair informações específicas sobre pessoas

Use o recurso de [pessoa](../resources/person.md) e a API de pessoas para agregação de informações sobre uma pessoa em email, contatos e redes sociais. Os resultados são ordenados por seu relevância com base em vários relacionamentos de negócios, colaboração e comunicação. A API permite procurar, classificar, selecione, filter ou pesquisa para as pessoas com base nos seus critérios.

- [Listar pessoas](../api/user-list-people.md)

## <a name="manage--mentions"></a>Gerenciar @ menções

Chamar check-out de um destinatário notificar e obter atenção do destinatário em uma mensagem é um gesto social comuns.
O recurso [mencionar](../resources/mention.md) e a API menções fornecem um mecanismo leve para destacar um destinatário em uma [mensagem](../resources/message.md), fazer todas as mensagens nas quais um usuário é notificado usando um @-mencionam ou fazer cada mencionam em uma mensagem.

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- Criar menções em uma nova mensagem

  - [Criar e enviar menções como parte de uma nova mensagem](../api/user-sendmail.md#request-2)
  - [Criar menções como parte de um rascunho de mensagem](../api/user-post-messages.md#request-2)

- Obter informações sobre menções em uma mensagem

  - [Obtenha todas as mensagens na caixa de correio do usuário conectado que mencionam o usuário](../api/user-list-messages.md#request-2)
  - [Obter detalhes de cada menção em uma mensagem](../api/message-get.md#request-2)

- [Excluir um mencionam](../api/message-delete.md#request-2) em uma mensagem

## <a name="access-social-data-around-and-about-a-user"></a>Acessar dados sociais ao redor e sobre um usuário

Gráfico do Office encapsula as relações entre as entidades diferentes no Office 365. Use o gráfico do Office para obter a ideias social para usuários individuais entre o Office 365.

- Listar os itens [tendências em torno de](../api/insights-list-trending.md) um usuário
- Listar usuários que tiverem sido [Trabalhando com](../api/user-list-people.md) um usuário
