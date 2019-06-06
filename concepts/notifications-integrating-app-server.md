---
title: Criar e enviar uma notificação do serviço de aplicativo
description: 'Configure o serviço de aplicativo para enviar notificações centradas no usuário para vários clientes por meio do Microsoft Graph. '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: cf40087aff3956a88f79197482db8126bbe8d96c
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34683507"
---
# <a name="create-and-send-a-notification-from-your-app-service"></a>Criar e enviar uma notificação do serviço de aplicativo

Você pode criar e enviar uma notificação para um usuário com as APIs do Microsoft Graph. As notificações são armazenadas no repositório de feed das atividades e enviadas a todos os clientes de aplicativos, em todos os dispositivos em que o usuário de destino está conectado. 

## <a name="authentication"></a>Autenticação

As notificações do Microsoft Graph exige que o serviço de aplicativo use o fluxo On-Behalf-Of (OBO) para postar uma notificação ao usuário. O fluxo de autenticação é o demonstrado a seguir::

1.  O usuário entra no aplicativo com a conta corporativa ou de estudante da Microsoft. Ao entrar, o serviço de identidade concede um token de acesso.

2.  Você envia o token de acesso ao serviço do aplicativo.

3.  O serviço do aplicativo autentica no serviço de identidade e solicita um token OBO para as notificações do Microsoft Graph.

4.  O serviço de identidade retorna um token com base em OBO e um token de atualização. O serviço de aplicativo pode usar o token de acesso para postar notificações ao usuário.

Para saber mais sobre o fluxo OAuth 2.0 OBO, consulte [Chamadas de serviço a serviço que usam a identidade do usuário delegado no fluxo On-Behalf-Of](https://docs.microsoft.com/pt-BR/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow). Para saber mais sobre como esse fluxo funciona com as notificações do Microsoft Graph, confira o [exemplo de serviço do aplicativo](https://aka.ms/gnsample-appservice).

> [!NOTE]
> As notificações do Microsoft Graph usa atualmente o fluxo de autenticação OBO com planos futuros para simplificar essa autenticação e acabar com a necessidade de manter tokens de acesso e tokens de atualização.

Para mais detalhes sobre as permissões de API e cabeçalhos de solicitação e resposta, veja [Criar e enviar notificação](/graph/api/notifications-post) na seção de referência do API. 
