---
title: 'Usar a API de notificações do Microsoft Graph para habilitar experiências de notificação centradas em humanos '
description: 'As notificações são a maneira mais eficaz de voltar a envolver os usuários. Eles podem chamam a atenção de seus usuários e trazê-los de volta para o aplicativo. Em um mundo de vários dispositivos, seus usuários podem acessar seus aplicativos e serviços em qualquer lugar e em diferentes plataformas e dispositivos nos quais os aplicativos estão presentes. '
ms.openlocfilehash: 7ff36d7e0d406cb7918e2999812e3c756ae3b5bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091590"
---
# <a name="using-the-notifications-api-in-microsoft-graph-to-enable-human-centric-notification-experiences"></a>Usar a API de notificações do Microsoft Graph para habilitar experiências de notificação centradas em humanos 

As notificações são a maneira mais eficaz de voltar a envolver os usuários. Eles podem chamam a atenção de seus usuários e trazê-los de volta para o aplicativo. Em um mundo de vários dispositivos, seus usuários podem acessar seus aplicativos e serviços em qualquer lugar e em diferentes plataformas e dispositivos nos quais os aplicativos estão presentes. 

Seus cenários de notificação devem ser projetados de modo centrado em humanos, em que a principal meta é notificar o usuário, onde quer que ele esteja. Soluções de notificação existentes fornecidas pelas principais plataformas são excelentes para direcionar a dispositivos. As notificações do Microsoft Graph melhoram isso, permitindo a você direcionar a usuários. As notificações do Microsoft Graph cuidarão do trabalho pesado, incluindo o mapeamento entre usuários e pontos de extremidade, sincronizando o estado de notificação em pontos de extremidade diferentes dos usuários e muito mais. 

## <a name="why-integrate-with-microsoft-graph-notifications"></a>Por que se integrar às notificações do Microsoft Graph?
### <a name="deliver-notifications-to-a-user-across-different-endpoints"></a>Entregar notificações a um usuário em pontos de extremidade diferentes
Como parte do Microsoft Graph, a API de notificações permite que você direcione para uma conta Microsoft ou uma conta corporativa ou de estudante (Azure AD) para entregar uma notificação. A plataforma distribui essa notificação aos pontos de extremidade de todos os usuários, incluindo UWP do Windows, Android e iOS. 

### <a name="manage-notifications-across-endpoints"></a>Gerenciar as notificações entre pontos de extremidade
A API de notificações do Microsoft Graph permite atualizar o estado de uma notificação e sincronizar o estado em todos os pontos de extremidade. Por exemplo, quando um usuário age sobre uma notificação em um dispositivo, você pode atualizar o estado essa notificação (por exemplo, marcá-la como lida ou ignorada), e essa alteração de estado será distribuída a todos os outros pontos de extremidade. A API de notificações do Microsoft Graph controla o estado das notificações de seus usuários de maneira centralizada, tornando fácil garantir que as notificações sejam manipuladas uma vez e ignoradas em todos os lugares.

### <a name="retrieve-notification-history"></a>Recuperar o histórico de notificações
Você pode usar a API de notificações para recuperar o histórico de notificações, com base em um período de expiração que você define (até 30 dias). Notificações marcadas como lidas ou ignoradas ainda são recuperáveis do histórico, permitindo exibições de histórico de notificações e de outros cenários no aplicativo. 

## <a name="integrating-with-the-notifications-api-in-microsoft-graph"></a>Integração com a API de notificações no Microsoft Graph

Os aplicativos podem ser integrados com notificações do Microsoft Graph com algumas etapas simples: integre seu aplicativo por meio do Centro de Desenvolvimento do Windows, use o método [Criar notificação](/graph/api/projectrome-notification-post?view=graph-rest-beta) para publicar notificações e use o SDK do projeto Roma para receber e gerenciar notificações em seus clientes do aplicativo.  

Para saber mais sobre como publicar notificações ao usuário por meio do Microsoft Graph, veja a [referência da API de notificações](/graph/api/resources/notifications-api-overview?view=graph-rest-beta).
 
Para saber mais sobre como receber e gerenciar as notificações por meio da integração com o SDK do projeto Roma, confira a [documentação do SDK do projeto Roma](https://docs.microsoft.com/pt-BR/windows/project-rome/) 

## <a name="see-also"></a>Confira também

- [Experiências entre dispositivos no Microsoft Graph](cross-device-concept-overview.md)
- [Centro de Desenvolvimento do projeto Roma](https://aka.ms/projectrome)
