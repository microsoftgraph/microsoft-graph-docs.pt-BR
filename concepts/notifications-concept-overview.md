---
title: 'Usando as notificações de API no Microsoft Graph para habilitar a notificação centrados em humanos experiências '
description: 'As notificações são a maneira mais eficaz entrem novamente a seus usuários. Eles podem chamar atenção dos usuários e trazer o usuário volta para seu aplicativo. Em um mundo de vários dispositivo, os usuários podem acessar seus aplicativos e serviços de qualquer lugar, em diferentes plataformas e dispositivos onde seus aplicativos tem uma presença. '
ms.openlocfilehash: 7ff36d7e0d406cb7918e2999812e3c756ae3b5bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091590"
---
# <a name="using-the-notifications-api-in-microsoft-graph-to-enable-human-centric-notification-experiences"></a>Usando as notificações de API no Microsoft Graph para habilitar a notificação centrados em humanos experiências 

As notificações são a maneira mais eficaz entrem novamente a seus usuários. Eles podem chamar atenção dos usuários e trazer o usuário volta para seu aplicativo. Em um mundo de vários dispositivo, os usuários podem acessar seus aplicativos e serviços de qualquer lugar, em diferentes plataformas e dispositivos onde seus aplicativos tem uma presença. 

Seus cenários de notificação devem ser projetados de forma "centrados em humanos", no qual o principal objetivo é notificar o usuário, onde quer que ele está. As soluções existentes de notificação são fornecidas pelo principais plataformas são excelentes no direcionamento de dispositivos. Notificações do Microsoft Graph melhoram nisso, permitindo aos usuários de destino. Notificações do Microsoft Graph executarão do trabalho pesado, incluindo o mapeamento entre usuários e pontos de extremidade, estado de notificação está sincronizando entre pontos de extremidade diferentes dos usuários e muito mais. 

## <a name="why-integrate-with-microsoft-graph-notifications"></a>Por que se integra com notificações do Microsoft Graph?
### <a name="deliver-notifications-to-a-user-across-different-endpoints"></a>Fornecer notificações para um usuário entre pontos de extremidade diferentes
Como parte do Microsoft Graph, a API de notificações permite que você direcione uma conta da Microsoft ou um trabalho ou escola conta (Azure AD) para fornecer uma notificação. A plataforma distribui essa notificação aos pontos de extremidade de todos os usuários, incluindo Windows UWP, Android e iOS. 

### <a name="manage-notifications-across-endpoints"></a>Gerenciar notificações entre pontos de extremidade
A API do Microsoft Graph notificações permite que você o estado de uma notificação de atualização e sincronize esse estado entre todos os pontos de extremidade. Por exemplo, quando um usuário atua em uma notificação em um dispositivo, você poderá atualizar o estado dessa notificação (por exemplo, marcá-la como lidos ou Prescindir) e a mesma alteração de estado será distribuída para todos os outros pontos de extremidade. A API do Microsoft Graph notificações rastreia o estado de notificações dos usuários de forma centralizada, tornando mais fácil de garantir que notificações são manipuladas uma vez e descartadas em todos os lugares.

### <a name="retrieve-notification-history"></a>Recuperar o histórico de notificação
Você pode usar as notificações de API para recuperar o histórico de notificação com base em uma data de vencimento que você define (até 30 dias). Notificações que são marcadas como ler ou descartado são ainda recuperáveis do histórico, habilitando os modos de exibição no aplicativo do histórico de notificação e outros cenários. 

## <a name="integrating-with-the-notifications-api-in-microsoft-graph"></a>Integrando com as notificações de API no Microsoft Graph

Você pode integrar seus aplicativos com notificações do Microsoft Graph com algumas etapas simples - integrado seu aplicativo por meio do Centro de desenvolvimento do Windows, use o método de [notificação de criar](/graph/api/projectrome-notification-post?view=graph-rest-beta) publique notificações e usar o SDK do Project Roma para receber e gerenciar notificações nos clientes app.  

Para saber mais sobre como publicar notificações de usuário por meio do Microsoft Graph, consulte a [referência de API de notificações](/graph/api/resources/notifications-api-overview?view=graph-rest-beta).
 
Para saber mais sobre como receber e gerenciando as notificações por meio da integração com o SDK do Project Roma, consulte a [documentação do SDK do Project Roma](https://docs.microsoft.com/en-us/windows/project-rome/) 

## <a name="see-also"></a>Confira também

- [Experiências entre dispositivos no Microsoft Graph](cross-device-concept-overview.md)
- [Centro de desenvolvimento do Project Roma](https://aka.ms/projectrome)
