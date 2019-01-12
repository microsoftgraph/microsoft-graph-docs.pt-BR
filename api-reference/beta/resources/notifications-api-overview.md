---
title: Usar as API REST de notificações no Microsoft Graph
description: Você pode usar as notificações de API no Microsoft Graph para enviar notificações por push para um usuário. Simplesmente uma conta de usuário para enviar uma notificação de destino e a plataforma representará uma notificação para todos os pontos de extremidade do dispositivo. Solicitações de notificações de API são realizadas em nome de um usuário por meio de permissões delegadas e a [permissão de notificação]( /graph/permissions_reference), que pode ser usado com um dos contas da Microsoft ou contas de trabalho ou da escola.
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 68a20b655eecea7d5afb82677178593b094a9cc3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931493"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Usar as API REST de notificações no Microsoft Graph

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Você pode usar as notificações de API no Microsoft Graph para enviar notificações por push para um usuário. Simplesmente uma conta de usuário para enviar uma notificação de destino e a plataforma representará uma notificação para todos os pontos de extremidade do dispositivo. Solicitações de notificações de API são realizadas em nome de um usuário por meio de [permissões delegadas](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) e a [permissão de notificação]( /graph/permissions_reference), que pode ser usado com um dos contas da Microsoft ou contas de trabalho ou da escola.
Esse tipo de notificação centrados no usuário é representado pelo recurso de [notificação](../resources/projectrome-notification.md) e é armazenado no Microsoft Graph. Ele pode ser acessado e gerenciado pelo publicação app por meio das [APIs do projeto Roma SDK](https://github.com/Microsoft/project-rome). 

## <a name="next-steps"></a>Próximas etapas
- Consulte o [recurso de notificação](../resources/projectrome-notification.md) e crie notificações se comprometer com seus usuários. 
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
