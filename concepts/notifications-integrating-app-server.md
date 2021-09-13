---
title: Criar e enviar uma notificação do serviço de aplicativo
description: 'Configure o serviço de aplicativo para enviar notificações centradas no usuário para vários clientes por meio do Microsoft Graph. '
ms.localizationpriority: high
ms.prod: notifications
author: merzink
ms.openlocfilehash: 24cac26e548d5f05724ee38559f6ef3bb4801277
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062317"
---
# <a name="create-and-send-a-notification-from-your-app-service"></a>Criar e enviar uma notificação do serviço de aplicativo

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
