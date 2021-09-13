---
title: Visão geral da API de aplicativos
description: Registre seu aplicativo com o Azure AD para criar uma configuração de identidade para ele que permita a integração com o Azure AD.
author: davidmu1
ms.localizationpriority: high
ms.prod: applications
ms.custom: scenarios:getting-started
ms.openlocfilehash: 6aef637d7e24e1d023012d81a365766cd7b6625e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59028748"
---
# <a name="applications-api-overview"></a>Visão geral da API de aplicativos

Para delegar as funções de gerenciamento de identidades e de acesso ao Azure AD, um aplicativo deve ser registrado em um locatário do Azure AD. Ao registrar seu aplicativo com o Azure AD, você está criando uma configuração de identidade para o aplicativo que permite a integração com o Azure AD.

## <a name="why-use-applications-and-associated-resources"></a>Por que usar aplicativos e recursos associados?

As APIs do Microsoft Graph permitem gerenciar esses recursos e ações relacionadas a aplicativos no Azure Active Directory:
- **Gerenciamento de aplicativos**: o Azure AD deve ser configurado para se integrar a um aplicativo. Em outras palavras, ele precisa saber quais aplicativos o estão usando como um sistema de identidade. O processo de manter o Azure AD ciente desses aplicativos e como ele deve tratá-los, é conhecido como gerenciamento de aplicativos.
- **Publicação local**: agentes locais (ou conectores para proxy de aplicativo) instalados por um administrador de locatários podem ser configurados para direcionar solicitações a um recurso publicado em particular.
- **Gerenciamento de entidade de serviço**: a representação local ou instância do aplicativo de um objeto de aplicativo global em um único locatário ou diretório. Uma entidade de serviço é uma instância concreta criada a partir do objeto do aplicativo e herda determinadas propriedades desse objeto do aplicativo.
- **Sincronização**: a sincronização de identidades do Azure Active Directory (Azure AD) (também chamada de *provisionamento*) permite automatizar a criação, a manutenção e a remoção de identidades na nuvem.

## <a name="application-management"></a>Gerenciamento de aplicativo

O registro do aplicativo envolve informar o Azure AD sobre seu aplicativo, incluindo a URL onde ele está localizado, a URL para enviar respostas após a autenticação, o URI para identificar seu aplicativo e muito mais. Você pode usar os [APIs de aplicativo](/graph/api/resources/application?view=graph-rest-1.0) no Microsoft Graph para gerenciar aplicativos programaticamente.

> [!VIDEO https://www.youtube-nocookie.com/embed/93j0MmRruFo]

Para obter mais informações sobre aplicativos, consulte os seguintes artigos:
- [Modelo de aplicativo](/azure/active-directory/develop/application-model)
- [Aplicativo e objetos de entidade de serviço no Azure Active Directory](/azure/active-directory/develop/app-objects-and-service-principals)
- [Tipos de aplicativo para a plataforma de identidade da Microsoft](/azure/active-directory/develop/v2-app-types)

Para obter mais informações sobre o gerenciamento de aplicativos, confira os artigos a seguir:
- [O que é o gerenciamento de aplicativo?](/azure/active-directory/manage-apps/what-is-application-management)
- [Fluxos de autenticação e cenários de aplicativos](/azure/active-directory/develop/authentication-flows-app-scenarios)

## <a name="on-premises-publishing-preview"></a>Publicação local (visualização)

Criar e gerenciar perfis de publicação locais, que inclui a criação de agentes locais e grupos de agentes. Você pode usar as [APIs de publicação local](/graph/api/resources/onpremisespublishingprofile-root) no Microsoft Graph para gerenciar perfis de publicação locais programaticamente.

Para obter mais informações sobre publicação no local, confira os artigos a seguir:
- [Acesso remoto a aplicativos locais por meio do proxy de Aplicativo Azure Active Directory](/azure/active-directory/manage-apps/application-proxy)
- [Usando o proxy do Aplicativo Azure AD para publicar aplicativos locais para usuários remotos](/azure/active-directory/manage-apps/what-is-application-proxy)

Para saber mais sobre como usar as APIs de publicação no local, confira o seguinte tutorial e suas APIs associadas:
- [Automatizar a configuração do Proxy de aplicativo usando a API do Microsoft Graph](./application-proxy-configure-api.md)
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [application](/graph/api/resources/application?view=graph-rest-1.0)
    - [onPremisesPublishing](/graph/api/resources/onpremisespublishingprofile-root)
    - [connector](/graph/api/resources/connector)
    - [connectorGroup](/graph/api/resources/connectorgroup)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="service-principal-management"></a>Gerenciamento da entidade de serviço

Para acessar os recursos que estão protegidos por um locatário do Azure AD, a entidade que exige o acesso deve ser representada por uma entidade de segurança. Você pode usar as [APIs da entidade de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) no Microsoft Graph para gerenciar entidades de serviço programaticamente.

Para obter mais informações sobre entidades de serviço, confira [Objetos de Aplicativo e de entidade de serviço no Azure Active Directory](/azure/active-directory/develop/app-objects-and-service-principals).

## <a name="synchronization"></a>Sincronização

Você pode usar as [APIs de sincronização ](/graph/api/resources/synchronization-overview) no Microsoft Graph para gerenciar a sincronização de identidade programaticamente, incluindo:
- Criar, iniciar e interromper trabalhos de sincronização
- Fazer alterações no esquema de sincronização para trabalhos
- Status de sincronização atual.

Para obter mais informações sobre a sincronização, consulte os seguintes artigos:
- [Automação do provisionamento e desprovisionamento de usuários para aplicativos com o Azure AD](/azure/active-directory/app-provisioning/user-provisioning)
- [Como funciona o provisionamento](/azure/active-directory/app-provisioning/how-provisioning-works)

Para saber mais sobre como usar as APIs de sincronização, confira os seguintes tutoriais e suas APIs associadas:
- [Configurar o provisionamento usando as APIs do Microsoft Graph](/azure/active-directory/app-provisioning/application-provisioning-configure-api)
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [synchronizationtemplate](/graph/api/resources/synchronization-synchronizationtemplate)
    - [synchronizationJob](/graph/api/resources/synchronization-synchronizationjob)
- [Automação da configuração do aplicativo de SSO baseado em SAML com a API do Microsoft Graph](/azure/active-directory/manage-apps/application-saml-sso-configure-api)
    - [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-1.0)
    - [application](/graph/api/resources/application?view=graph-rest-1.0)
    - [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy)
    - [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)

## <a name="next-steps"></a>Próximas etapas
- Experimente a API do Microsoft Graph no[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer). 
- Saiba mais sobre como adicionar autenticação e autorização aos aplicativos Web e às APIs da Web usando [estes exemplos](/azure/active-directory/develop/sample-v2-code).
