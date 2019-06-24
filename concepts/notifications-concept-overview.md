---
title: 'Ativando experiências de notificação centradas no ser humano usando notificações do Microsoft Graph '
description: 'As notificações são uma das maneiras mais eficazes de se envolver novamente com os usuários do seu aplicativo. Uma ótima experiência de notificação pode ajudar a abrir um canal de comunicação quase em tempo real entre você e os usuários do aplicativo, o que pode aumentar o engajamento com o aplicativo no momento certo, ajudar os usuários a serem mais produtivos e alertá-los sobre eventos importantes ou ações oportunas que possam ser necessárias. '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: b83e91be74de44dbd72315331964379992b811de
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133562"
---
# <a name="enabling-human-centric-notification-experiences-using-microsoft-graph-notifications"></a>Ativando experiências de notificação centradas no ser humano usando notificações do Microsoft Graph

As notificações são uma das formas mais eficazes de interagir com os usuários do seu aplicativo. Uma ótima experiência de notificação pode ajudar a abrir um canal de comunicação quase em tempo real entre você e seus usuários, o que pode aumentar o engajamento com o aplicativo no momento certo, tornar os usuários mais produtivos e alertá-los sobre eventos importantes ou ações necessárias.

> [!VIDEO https://www.youtube-nocookie.com/embed/cmpPFhrS8ZA]

Hoje, os usuários podem acessar seus aplicativos e serviços por meio de uma ampla variedade de plataformas e formatos. Essa combinação de dispositivos exige que você entenda e dê suporte a sistemas de notificação multiplataforma, mapeie usuários para pontos de extremidade e mantenha o estado de notificação em todos os dispositivos. 

A maioria dos outros sistemas de notificação elimina a necessidade de entender e direcionar sistemas de notificação por push específicos da plataforma, mas ainda são projetados para cada dispositivo. As notificações do Microsoft Graph fornecem uma abordagem centrada no ser humano que oferece a capacidade de direcionar seus usuários em todos os pontos de extremidade de dispositivos.

![Uma imagem que mostra um serviço de aplicativo se comunicando com o Microsoft Graph para enviar notificações para vários pontos de extremidade](images/notifications-flow-overview.png)

## <a name="why-integrate-with-microsoft-graph-notifications"></a>Por que se integrar às notificações do Microsoft Graph?

As notificações do Microsoft Graph fornecem uma plataforma de notificação centrada no usuário que traz quatro benefícios principais para seus aplicativos.

### <a name="effortlessly-target-your-user-for-notification-delivery-across-different-endpoints"></a>Direcione sem esforço seu usuário para o fornecimento de notificações em diferentes pontos de extremidade

Você pode usar a API de notificações para direcionar uma conta pessoal da Microsoft ou uma conta do Azure Active Directory (Azure AD) corporativa ou de estudante para fornecer notificações. A plataforma distribui essa notificação para todos os pontos de extremidade de usuários que executam seu aplicativo ou serviço, incluindo o Windows UWP, o Android e o iOS. Esse recurso ajuda a maximizar o alcance, garantindo que as notificações apropriadas possam alcançar seu destino, onde quer que estejam.

### <a name="easily-manage-notifications-across-endpoints"></a>Gerencie as notificações facilmente pelos pontos de extremidade

Usando o [SDK do cliente de notificações do Microsoft Graph](https://github.com/microsoft/project-rome) em seu aplicativo cliente, você pode atualizar o estado de uma notificação e sincronizá-lo em todos os pontos de extremidade. Por exemplo, quando um usuário age sobre uma notificação em um dispositivo, você pode atualizar o estado essa notificação (por exemplo, marcá-la como lida ou ignorada), e essa alteração de estado será distribuída a todos os outros pontos de extremidade. A API de notificações do Microsoft Graph acompanha o estado das notificações do usuário de forma centralizada, facilitando a garantia de que suas notificações sejam tratadas uma vez e descartadas em todo lugar, minimizando a redundância e garantindo uma excelente experiência do cliente.

### <a name="retrieve-notification-state-and-history"></a>Recuperar estado e histórico de notificação

Você pode usar a API de notificações para recuperar o histórico de notificações, com base em um período de expiração que você define (até 30 dias). As notificações marcadas como lidas ou dispensadas ainda podem ser recuperadas do histórico, permitindo visualizações no aplicativo do histórico de notificações, além de permitir que você desenvolva insights e inteligência.

### <a name="privacy-and-compliance"></a>Privacidade e conformidade

As notificações do Microsoft Graph atendem à maioria dos requisitos de conformidade corporativa, incluindo ISO 27001, ISO 27018, EUMC, HIPAA, SOC 1, SOC 2 e, é claro, GDPR.

## <a name="how-do-i-get-started"></a>Por onde começar?

Para começar, consulte a seção de [visão geral da integração](notifications-integration-e2e-overview.md) para saber como integrar as notificações centradas no usuário em seu aplicativo.
