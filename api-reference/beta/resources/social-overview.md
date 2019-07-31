---
title: Usar a API do Microsoft Graph para integrar a inteligência social e do local de trabalho em um aplicativo
description: O Microsoft Graph dá suporte a gestos sociais em um contexto social do usuário e fornece acesso a pessoas e dados sociais úteis.
localization_priority: Priority
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 84e0c82173dad6f08d5911f32ef5c384f041ea19
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008086"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-and-workplace-intelligence-in-an-app"></a>Usar a API do Microsoft Graph para integrar a inteligência social e do local de trabalho em um aplicativo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Microsoft Graph dá suporte a gestos sociais em um contexto social do usuário e fornece acesso a pessoas e dados sociais úteis.

## <a name="aggregate-and-extract-specific-information-about-people"></a>Agregar e extraia informações específicas sobre pessoas

Use o recurso [person](../resources/person.md) e a API de Pessoas para agregar informações sobre uma pessoa provenientes de emails, contatos e redes sociais. Os resultados são ordenados por sua relevância com base em várias relações de comunicação, colaboração e comerciais. A API permite navegar, classificar, selecionar, filtrar ou procurar pessoas com base em critérios selecionados.

- [Listar pessoas](../api/user-list-people.md)

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a>Ajudar os usuários a obter os documentos mais relevantes para seu trabalho

Usar a API insights para identificar os documentos mais relevantes para o usuário: 

- Listar documentos [mais populares](../api/insights-list-trending.md) de um usuário
- Listar documentos [usados por](../api/insights-list-used.md) um usuário
- Listar documentos [compartilhados com ou por](../api/insights-list-shared.md) um usuário

## <a name="manage--mentions"></a>Gerenciar as @menções

Chamar um destinatário para notificar e atrair a atenção do destinatário em uma mensagem é um gesto social comum.
O recurso [menção](../resources/mention.md) e a API de Menções fornecem um mecanismo simplificado para marcar um destinatário em uma [mensagem](../resources/message.md), receber todas as mensagens nas quais um usuário é notificado usando uma @menção ou receber cada menção em uma mensagem.

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- Criar menções em uma nova mensagem

  - [Criar e enviar menções como parte de uma nova mensagem](../api/user-sendmail.md#request-2)
  - [Criar menções como parte de um rascunho da mensagem](../api/user-post-messages.md#request-2)

- Obter informações sobre menções em uma mensagem

  - [Obter todas as mensagens na caixa de correio do usuário conectado que mencionou o usuário](../api/user-list-messages.md#request-2)
  - [Obter os detalhes de cada menção em uma mensagem](../api/message-get.md#request-2)

- [Excluir uma menção](../api/message-delete.md#request-2) em uma mensagem

