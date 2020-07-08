---
title: Visão geral da API de aplicativos
description: Registre seu aplicativo com o Azure AD para criar uma configuração de identidade para ele que permita a integração com o Azure AD.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: scenarios:getting-started
ms.openlocfilehash: ff38e14182d2e38fbc2203241da911dec07f9846
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081190"
---
# <a name="applications-api-overview"></a>Visão geral da API de aplicativos

Para delegar funções de gerenciamento de identidades e acesso ao Azure AD, um aplicativo deve ser registrado em um locatário do Azure AD. Ao registrar seu aplicativo com o Azure AD, você está criando uma configuração de identidade para seu aplicativo que permite a integração com o Azure AD.

## <a name="why-use-applications-and-associated-resources"></a>Por que usar aplicativos e recursos associados?

As APIs do Microsoft Graph permitem que você gerencie esses recursos e ações relacionadas aos aplicativos no Azure Active Directory:
- **Gerenciamento de aplicativos** – o Azure ad deve ser configurado para integração com um aplicativo. Em outras palavras, ele precisa saber quais aplicativos estão usando-o como um sistema de identidade. O processo de manter o Azure AD ciente desses aplicativos e como ele deve tratá-los, é conhecido como gerenciamento de aplicativos.
- Agentes de **publicação** local (ou conectores de proxy de aplicativo) instalados por um administrador de locatários podem ser configurados para encaminhar solicitações a um determinado recurso publicado.
- **Gerenciamento de entidade de serviço** -a representação local, ou instância de aplicativo, de um objeto de aplicativo global em um único locatário ou diretório. Uma entidade de serviço é uma instância concreta criada a partir do objeto Application e herda determinadas propriedades desse objeto Application.
- **Sincronização** -a sincronização de identidade do Azure Active Directory (Azure AD) (também chamada de *provisionamento*) permite automatizar a criação, a manutenção e a remoção de identidades na nuvem.

## <a name="application-management"></a>Gerenciamento de aplicativo

O registro do aplicativo envolve informar o Azure AD sobre seu aplicativo, incluindo a URL onde ele está localizado, a URL para enviar respostas após a autenticação, o URI para identificar seu aplicativo e muito mais. Você pode usar as [APIs de aplicativo](/graph/api/resources/application?view=graph-rest-1.0) no Microsoft Graph para gerenciar aplicativos programaticamente.

> [!VIDEO https://www.youtube-nocookie.com/embed/93j0MmRruFo]

Para obter mais informações sobre aplicativos, consulte os seguintes artigos:
- [Modelo de aplicativo](https://docs.microsoft.com/azure/active-directory/develop/application-model)
- [Aplicativo e objetos de entidade de serviço no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
- [Tipos de aplicativos para a plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-app-types)

Para obter mais informações sobre o gerenciamento de aplicativos, consulte os seguintes artigos:
- [O que é gerenciamento de aplicativos?](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-application-management)
- [Fluxos de autenticação e cenários de aplicativos](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios)

## <a name="on-premises-publishing-preview"></a>Publicação local (visualização)

Criar e gerenciar perfis de publicação local, que incluem a criação de agentes locais e grupos de agentes. Você pode usar as [APIs de publicação local](/graph/api/resources/onpremisespublishingprofile-root) no Microsoft Graph para gerenciar perfis de publicação no local programaticamente.

Para obter mais informações sobre publicação local, consulte os seguintes artigos:
- [Acesso remoto para aplicativos locais por meio do proxy de aplicativo do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy)
- [Usando o proxy de aplicativo do Azure AD para publicar aplicativos locais para usuários remotos](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-application-proxy)

Para saber mais sobre como usar as APIs de publicação local, consulte o seguinte tutorial e suas APIs associadas:
- [Automatizar a configuração do proxy de aplicativo usando a API do Microsoft Graph](https://docs.microsoft.com/graph/application-proxy-configure-api)
    - [applicationtemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [aplicativo](/graph/api/resources/application?view=graph-rest-1.0)
    - [onPremisesPublishing](/graph/api/resources/onpremisespublishingprofile-root)
    - [conector](/graph/api/resources/connector)
    - [connectorGroup](/graph/api/resources/connectorgroup)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="service-principal-management"></a>Gerenciamento da entidade de serviço

Para acessar os recursos que são protegidos por um locatário do Azure AD, a entidade que requer acesso deve ser representada por uma entidade de segurança. Você pode usar as [APIs de entidade de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) no Microsoft Graph para gerenciar entidades de segurança de serviço programaticamente.

Para obter mais informações sobre entidades de serviço, consulte [Application and Service principal Objects in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).

## <a name="synchronization"></a>Sincronização

Você pode usar as [APIs de sincronização](/graph/api/resources/synchronization-overview) no Microsoft Graph para gerenciar a sincronização de identidade de forma programática, incluindo:
- Criar, iniciar e interromper trabalhos de sincronização
- Fazer alterações no esquema de sincronização para trabalhos
- Verificar o status de sincronização atual

Para obter mais informações sobre sincronização, consulte os seguintes artigos:
- [Automatizar o provisionamento de usuários e desprovisionamento para aplicativos com o Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)
- [Como o provisionamento funciona](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works)

Para saber mais sobre como usar as APIs de sincronização, consulte os seguintes tutoriais e suas APIs associadas:
- [Configurar o provisionamento usando as APIs do Microsoft Graph](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api)
    - [applicationtemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [synchronizationtemplate](/graph/api/resources/synchronization-synchronizationtemplate)
    - [synchronizationJob](/graph/api/resources/synchronization-synchronizationjob)
- [Automatizar a configuração do aplicativo SSO baseado em SAML com a API do Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api)
    - [applicationtemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [aplicativo](/graph/api/resources/application?view=graph-rest-1.0)
    - [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="next-steps"></a>Próximas etapas
- Experimente a API do Microsoft Graph no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Saiba como adicionar autenticação e autorização aos aplicativos Web e APIs Web usando [esses exemplos](https://docs.microsoft.com/azure/active-directory/develop/sample-v2-code).
