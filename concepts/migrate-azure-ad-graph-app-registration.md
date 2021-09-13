---
title: Revisar o registro de aplicativos, permissões e problemas de migração de consentimento
description: Descreve a migração de registro, permissão e consentimento do aplicativo Azure Active Directory (Azure AD) para a API Graph Microsoft.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: e6b4746d5928bd56057e4aacf91eafea5cad5e90
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117652"
---
# <a name="review-app-registration-permissions-and-consent"></a>Revisar o registro, permissões e consentimento do aplicativo

Este artigo faz parte da *etapa 3:* revisar detalhes do aplicativo do [processo para migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

Para qualquer atualização de aplicativo, há três áreas a considerar:

- **Registro de** aplicativo : você pode continuar a usar seu registro de aplicativo existente ( `appId` ) no código do aplicativo.  

    Você não **precisa** registrar seu aplicativo para migrar para o Microsoft Graph. Basta atualizar o código, testar fortemente e implantar a atualização.  

- Permissões : Você deve alterar suas permissões configuradas para as permissões **equivalentes** Graph Microsoft. Permissões delegadas que foram concedidas para Azure Active Directory (Azure AD) Graph serão implicitamente consideradas concedidas para o Microsoft Graph também. Permissões de aplicativo (funções de aplicativo) precisarão ser concedidas novamente.

    Se sua atualização também inscui o uso de recursos ou recursos que não estão disponíveis para o Azure AD Graph, você provavelmente precisará solicitar permissões para esses novos recursos. Se esse for o caso, você pode alternar seu aplicativo para usar o MSAL e o ponto de extremidade v2 e solicitar o consentimento adicional/incremental dinamicamente. Encontre mais detalhes sobre como alternar para o MSAL em revisar alterações na biblioteca [de autenticação de aplicativos.](./migrate-azure-ad-graph-authentication-library.md)

- **Consentimento**: Os usuários finais que já concederam consentimento para permissões delegadas (ou para quem o consentimento já foi concedido por um administrador) podem continuar usando seu aplicativo sem ser solicitado a conceder consentimento novamente.

    Os usuários que já concederam consentimento ao seu aplicativo para acessar seus dados podem continuar a usar seu aplicativo depois que ele tiver sido atualizado para usar o Microsoft Graph, sem ser solicitado a consentir novamente. Novos usuários serão solicitados a consentir.

Projetos de migração simples não devem ter problemas nessas áreas.

No entanto, se você usar novos recursos, serviços ou adicionar recursos adicionais, poderá precisar de novas permissões e o consentimento do usuário final pode ser necessário.  Nesses casos, o consentimento é solicitado quando os tokens são atualizados.

## <a name="next-steps"></a>Próximas etapas

- Saiba [as diferenças de biblioteca](migrate-azure-ad-graph-authentication-library.md) de autenticação entre o Azure AD Graph e o Microsoft Graph.
- Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.
