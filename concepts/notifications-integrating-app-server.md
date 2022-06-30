---
title: Criar e enviar uma notificação do seu serviço de aplicativo (preterido)
description: Você pode criar e enviar uma notificação para um usuário com as APIs do Microsoft Graph (preterido).
ms.localizationpriority: high
ms.prod: notifications
author: merzink
ms.openlocfilehash: 302375137bb2408bcd6be5ad737cf34cc7d6ee70
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447132"
---
# <a name="create-and-send-a-notification-from-your-app-service-deprecated"></a>Criar e enviar uma notificação do seu serviço de aplicativo (preterido)

> [!IMPORTANT]
> A API de notificações do Microsoft Graph foi preterida e parou de retornar dados em janeiro de 2022. Para uma experiência de notificação alternativa, confira os [Hubs de Notificações do Microsoft Azure](/azure/notification-hubs). Para obter mais informações, consulte a postagem no blog [Desativando a API de notificações do Microsoft Graph (beta)](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/).

Você pode criar e enviar uma notificação para um usuário com as APIs do Microsoft Graph. As notificações são armazenadas no repositório do serviço de Notificações do Microsoft Graph e enviadas a todos os clientes de aplicativos, em todos os dispositivos em que o usuário de destino está conectado. 

Para enviar uma notificação para o usuário, seu serviço de aplicativo precisará:
1. [Autenticar](/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) com a plataforma de identidade da Microsoft.
2. Publique uma notificação para a API do Microsoft Graph usando o token de autenticação e direcione o usuário com uma [ID de assinatura de notificação de usuário](/graph/api/notifications-post) que é obtida do seu cliente de aplicativo ao criar uma assinatura.

> [!NOTE]
> Para uma história de autenticação simplificada, recomendamos usar o novo e aprimorado [SDK de notificação](https://aka.ms/GNSDK) do lado do cliente com uma ID de assinatura de notificação de usuário para receber notificações e gerenciar o estado de notificação. Como alternativa, você pode publicar notificações em nome do usuário por meio de permissões delegadas e seu serviço de aplicativo precisará manter tokens de acesso e de atualização, mas isso não é recomendável. Para saber mais sobre o fluxo OAuth 2.0 OBO, confira [Chamadas de serviço a serviço que usam a identidade do usuário delegado no fluxo On-Behalf-Of](/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow). 


## <a name="guaranteed-delivery-on-ios"></a>Entrega garantida no iOS

Em plataformas como o iOS, em certas condições energéticas, a entrega de notificações de dados brutos pode atrasar devido ao processamento em lotes ou pode nem chegar ao ponto de extremidade. Para notificações com alta prioridade entregues a usuários no iOS, a plataforma de notificações do Microsoft Graph permite especificar uma opção de "fallback" de notificação do sistema "raw-to-visual" que envia automaticamente uma notificação do sistema visual para o dispositivo iOS de destino, garantindo que os usuários sejam notificados praticamente em tempo real. Para saber como aproveitar as opções de fallback, confira o [recurso de notificação](/graph/api/resources/projectrome-notification.md).  

## <a name="getting-started"></a>Introdução
Para saber como o seu serviço de aplicativo pode começar a enviar notificações aos seus usuários, confira [notificação](/graph/api/resources/projectrome-notification) e o nosso [Exemplo do serviço de aplicativo](https://aka.ms/gnsample-appservice).
