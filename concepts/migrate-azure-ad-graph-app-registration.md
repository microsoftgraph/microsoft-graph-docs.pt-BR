---
title: Revisar problemas de migração de registro, permissões e autorização de aplicativo
description: Descreve o registro de aplicativo, permissão e migração de consentimento do Azure Active Directory (Azure AD) para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 54e187fcf35f030413aa98a6cb0e34649532a8b4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630276"
---
# <a name="review-app-registration-permissions-and-consent"></a>Revisar o registro, as permissões e o consentimento do aplicativo

Este artigo faz parte da *etapa 3: revise os detalhes do aplicativo* do [processo para migrar aplicativos](migrate-azure-ad-graph-planning-checklist.md).

Para qualquer atualização de aplicativos, há três áreas que devem ser consideradas:

- **Registro do aplicativo**: você pode continuar a usar seu registro de aplicativo`appId`existente () no seu código de aplicativo.  

    Você **não** precisa registrar seu aplicativo novamente para migrar para o Microsoft Graph. Basta atualizar o código, testar fortemente e implantar sua atualização.  

- **Permissões**: você pode continuar a usar as permissões configuradas existentes para o seu aplicativo. Você não precisa solicitar novas permissões porque as permissões do Azure AD Graph são compartilhadas com o Microsoft Graph.

    Por exemplo, se o aplicativo existente tiver as permissões _User. Read. All_ e _Group. Read. All_ , essas permissões também serão implicitamente concedidas ao seu aplicativo atualizado para o Microsoft Graph.

    Se sua atualização também Incudes o uso de recursos ou recursos que não estão disponíveis para o Azure AD Graph, provavelmente você precisará solicitar permissões para esses novos recursos. Se esse for o caso, você pode mudar seu aplicativo para usar o MSAL e o ponto de extremidade V2 e solicitar o consentimento adicional/incremental dinamicamente. Encontre mais detalhes sobre a mudança para o MSAL em revisar [alterações na biblioteca de autenticação de aplicativos](/graph/migrate-azure-ad-graph-authentication-library).

- **Consentimento**: os usuários finais podem continuar usando o aplicativo sem precisar conceder o consentimento novamente.

    Os usuários que já concederam o consentimento do seu aplicativo para acessar seus dados podem continuar a usar seu aplicativo após ele ter sido atualizado para usar o Microsoft Graph, sem solicitar o consentimento.

Projetos de migração simples não devem ter problemas nessas áreas.

No entanto, se você usar novos recursos, serviços ou adicionar recursos adicionais, talvez precise de novas permissões e o consentimento do usuário final possa ser necessário.  Nesses casos, o consentimento é solicitado quando os tokens são atualizados.

## <a name="next-steps"></a>Próximos passos

- Saiba mais sobre as diferenças da [biblioteca de autenticação](migrate-azure-ad-graph-authentication-library.md) entre o Azure ad Graph e o Microsoft Graph.
- Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .
- Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.
