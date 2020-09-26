---
title: Revisar problemas de migração de registro, permissões e autorização de aplicativo
description: Descreve o registro de aplicativo, permissão e migração de consentimento do Azure Active Directory (Azure AD) para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 8cca43199d8549841087a84d1bd275e38f09efdb
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288340"
---
# <a name="review-app-registration-permissions-and-consent"></a>Revisar o registro, as permissões e o consentimento do aplicativo

Este artigo faz parte da *etapa 3: revise os detalhes do aplicativo* do [processo para migrar aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Para qualquer atualização de aplicativos, há três áreas que devem ser consideradas:

- **Registro do aplicativo**: você pode continuar a usar seu registro de aplicativo existente ( `appId` ) no seu código de aplicativo.  

    Você **não** precisa registrar seu aplicativo novamente para migrar para o Microsoft Graph. Basta atualizar o código, testar fortemente e implantar sua atualização.  

- **Permissões**: você pode continuar a usar as permissões configuradas existentes para o seu aplicativo. Você não precisa solicitar novas permissões porque as permissões do Azure AD Graph são compartilhadas com o Microsoft Graph.

    Por exemplo, se o aplicativo existente tiver as permissões _User. Read. All_ e _Group. Read. All_ , essas permissões também serão implicitamente concedidas ao seu aplicativo atualizado para o Microsoft Graph.

    Se sua atualização também Incudes o uso de recursos ou recursos que não estão disponíveis para o Azure AD Graph, provavelmente você precisará solicitar permissões para esses novos recursos. Se esse for o caso, você pode mudar seu aplicativo para usar o MSAL e o ponto de extremidade V2 e solicitar o consentimento adicional/incremental dinamicamente. Encontre mais detalhes sobre a mudança para o MSAL em [revisar alterações na biblioteca de autenticação de aplicativos](./migrate-azure-ad-graph-authentication-library.md).

- **Consentimento**: os usuários finais podem continuar usando o aplicativo sem precisar conceder o consentimento novamente.

    Os usuários que já concederam o consentimento do seu aplicativo para acessar seus dados podem continuar a usar seu aplicativo após ele ter sido atualizado para usar o Microsoft Graph, sem solicitar o consentimento.

Projetos de migração simples não devem ter problemas nessas áreas.

No entanto, se você usar novos recursos, serviços ou adicionar recursos adicionais, talvez precise de novas permissões e o consentimento do usuário final possa ser necessário.  Nesses casos, o consentimento é solicitado quando os tokens são atualizados.

## <a name="next-steps"></a>Próximas etapas

- Saiba mais sobre as diferenças da [biblioteca de autenticação](migrate-azure-ad-graph-authentication-library.md) entre o Azure ad Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.