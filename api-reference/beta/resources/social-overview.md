---
title: Usar a API do Microsoft Graph para integrar a inteligência de pessoas e de local de trabalho em um aplicativo
description: O Microsoft Graph permite o acesso a dados úteis sobre pessoas, seu perfil, documentos dos quais eles interagem e padrões de trabalho e oferece suporte a gestos no contexto social de um usuário.
ms.localizationpriority: high
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 460f5d4af2dbc75b9496b7ff0e5c33d9d62a7fd0
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461195"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-and-workplace-intelligence-in-an-app"></a>Usar a API do Microsoft Graph para integrar a inteligência de pessoas e de local de trabalho em um aplicativo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Microsoft Graph permite o acesso a dados úteis sobre pessoas, seu perfil, documentos dos quais eles interagem e padrões de trabalho e oferece suporte a gestos no contexto social de um usuário.

## <a name="aggregate-and-extract-specific-information-about-people"></a>Agregar e extraia informações específicas sobre pessoas

Recurso: Pessoas

Use o recurso [person](../resources/person.md) e a API de Pessoas para agregar informações sobre uma pessoa provenientes de emails, contatos e redes sociais. Os resultados são ordenados por sua relevância com base em várias relações de comunicação, colaboração e comerciais. A API permite navegar, classificar, selecionar, filtrar ou procurar pessoas com base em critérios selecionados.

- [Listar pessoas](../api/user-list-people.md)

## <a name="help-users-contextualize-others-in-their-organization"></a>Ajudar os usuários a contextualizarem outras pessoas em sua organização

Recurso: Perfil (visualização)

As pessoas que procuram contextualizar outras na organização geralmente exibem o perfil ou o cartão de perfil de uma pessoa.

O recurso [perfil](../resources/profile.md) é uma avançada fonte de informações sobre as pessoas dentro de um locatário e proporciona um mecanismo leve para armazenar e recuperar informações sobre alguém.

## <a name="personalize-people-experiences-within-your-organization"></a>Personalizar experiências de pessoas dentro da sua organização

Recurso: Personalização de cartão de perfil (visualização)

Oferece a capacidade de um administrador personalizar as informações mostradas no cartão de perfil usado no Microsoft 365 em sua organização.

O recurso [profileCardProperty](../resources/profileCardProperty.md) representa um atributo de um usuário no cartão de perfil do Microsoft 365 para uma organização ter uma experiência compartilhada por pessoas.

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a>Ajudar os usuários a obter os documentos mais relevantes para seu trabalho

Recurso: Ideias do documento

Usar a API insights para identificar os documentos mais relevantes para o usuário:

- Listar documentos [mais populares](../api/insights-list-trending.md) de um usuário
- Listar documentos [usados por](../api/insights-list-used.md) um usuário
- Listar documentos [compartilhados com ou por](../api/insights-list-shared.md) um usuário
- Explore maneiras de [personalizar as configurações de privacidade para obter informações sobre itens](/graph/insights-customize-item-insights-privacy) em uma organização.

## <a name="manage--mentions"></a>Gerenciar as @menções

Recurso: @-menções (visualização)

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


## <a name="help-users-gain-insights-into-their-work-patterns"></a>Ajudar os usuários a obter informações sobre seus padrões de trabalho

Recurso: Análise (visualização)

Usar a API de análise para obter estatísticas de atividade e configurações relacionadas para um usuários:

- [configurações](../resources/settings.md): Para a API de análise retornar os resultados para um usuário, as configurações de análise de usuário atual devem mostrar uma licença válida do Microsoft Viva Insights, ser optadas para usar o Viva Insights, e ter uma caixa de correio hospedada na nuvem habilitada para representar em gráfico.
- [activityStatistics](../resources/activitystatistics.md): Obtém dados da última semana concluída (ou do intervalo de tempo especificado) das atividades do Microsoft 365 nas quais um usuário passou algum tempo, incluindo o número de horas gastas em [chamadas](callactivitystatistics.md), [conversas (mensagens instantâneas)](chatactivitystatistics.md), [email](emailactivitystatistics.md) e [reuniões](meetingactivitystatistics.md) durante e fora das horas de trabalho e o número de horas disponíveis para o [trabalho prioritário](focusactivitystatistics.md).

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para esses conjuntos de API.


