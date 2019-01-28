---
title: Usar a API do Microsoft Graph para integrar a inteligência social em um aplicativo
description: O Microsoft Graph dá suporte a gestos sociais em um contexto social do usuário e fornece acesso a pessoas e dados sociais úteis.
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: b5a89f46c8480fb90cd019e5b4fb370e0a6592bf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509592"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a>Usar a API do Microsoft Graph para integrar a inteligência social em um aplicativo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Microsoft Graph dá suporte a gestos sociais em um contexto social do usuário e fornece acesso a pessoas e dados sociais úteis.

## <a name="aggregate-and-extract-specific-information-about-people"></a>Agregar e extraia informações específicas sobre pessoas

Use o recurso [person](../resources/person.md) e a API de Pessoas para agregar informações sobre uma pessoa provenientes de emails, contatos e redes sociais. Os resultados são ordenados por sua relevância com base em várias relações de comunicação, colaboração e comerciais. A API permite navegar, classificar, selecionar, filtrar ou procurar pessoas com base em critérios selecionados.

- [Listar pessoas](../api/user-list-people.md)

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

## <a name="access-social-data-around-and-about-a-user"></a>Acessar dados sociais em torno e sobre um usuário

O Office Graph encapsula as relações entre diferentes entidades no Office 365. Use o Office Graph para obter informações sociais sobre usuários individuais no Office 365.

- Listar os itens de [tendência em torno](../api/insights-list-trending.md) de um usuário
- Listar usuários que têm [trabalhado com](../api/user-list-people.md) um usuário
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/social-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
