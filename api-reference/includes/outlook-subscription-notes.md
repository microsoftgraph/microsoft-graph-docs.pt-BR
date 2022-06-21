---
author: angelgolfer-ms
ms.localizationpriority: high
ms.prod: outlook
ms.topic: include
ms.openlocfilehash: f790fd4357bfe63ad364fff30a7de0c69d94dfe0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333712"
---
<!-- markdownlint-disable MD041-->
Criar e gerenciar (obter, atualizar e excluir) uma assinatura requer um escopo de leitura para o recurso. Por exemplo, para receber notificações de alteração nas mensagens, seu aplicativo precisa da permissão Mail.Read. As notificações de alteração do Outlook dão suporte a escopos de permissão de aplicativo e delegados. Observe as seguintes limitações:

- A permissão delegada dá suporte a inscrição de itens em pastas apenas na caixa de correio do usuário conectado. Por exemplo, você não pode usar os Calendários de permissões delegadas. Leia para assinar eventos na caixa de correio de outro usuário.
- Se inscrever para alterar as notificações de contatos, eventos no Outlook ou mensagens em pastas _compartilhadas ou delegadas_:

  - Usar a permissão de aplicativos correspondentes para inscrever as alterações dos itens em uma pasta ou uma caixa de correio de _qualquer_ usuários no locatário.
  - Não use as permissões de compartilhamento do Outlook (Contacts.Read.Shared Calendars.Read.Shared, Mail.Read.Shared e seus equivalentes de somente leitura), pois eles **não** suportam inscrições que alteram as notificações em itens de pastas compartilhadas ou delegadas.