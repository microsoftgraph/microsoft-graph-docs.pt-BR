---
title: Visão geral da API de aplicativos
description: 'As APIs do Microsoft Graph permitem que você faça o seguinte no Azure AD: gerenciamento de aplicativos, publicação local, gerenciamento de entidade de serviço e sincronização.'
author: FaithOmbongi
ms.localizationpriority: high
ms.prod: applications
ms.custom: scenarios:getting-started
ms.openlocfilehash: 15bb312928eb3fe4810d3353d4e2d4c04b266be0
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095066"
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

O registro de aplicativo envolve informar ao Azure Active Directory sobre seu aplicativo, incluindo a URL onde ele está localizado, a URL para enviar respostas após a autenticação, a URI para identificar seu aplicativo e muito mais. Você pode usar as [APIs de aplicativo](/graph/api/resources/application) no Microsoft Graph gerenciar aplicativos programaticamente.

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
    - [applicationTemplate](/graph/api/resources/applicationtemplate)
    - [application](/graph/api/resources/application)
    - [onPremisesPublishing](/graph/api/resources/onpremisespublishingprofile-root)
    - [connector](/graph/api/resources/connector)
    - [connectorGroup](/graph/api/resources/connectorgroup)
    - [servicePrincipal](/graph/api/resources/serviceprincipal)

## <a name="service-principal-management"></a>Gerenciamento da entidade de serviço

Para acessar os recursos que estão protegidos por um locatário do Azure AD, a entidade que exige o acesso deve ser representada por uma entidade de segurança. Você pode usar as [APIs da entidade de serviço](/graph/api/resources/serviceprincipal) no Microsoft Graph para gerenciar entidades de serviço programaticamente.

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
- [Configurar o provisionamento usando as APIs do Microsoft Graph](/azure/active-directory/app-provisioning/application-provisioning-configuration-api)
    - [applicationTemplate](/graph/api/resources/applicationtemplate)
    - [synchronizationtemplate](/graph/api/resources/synchronization-synchronizationtemplate)
    - [synchronizationJob](/graph/api/resources/synchronization-synchronizationjob)
- [Automação da configuração do aplicativo de SSO baseado em SAML com a API do Microsoft Graph](/azure/active-directory/manage-apps/application-saml-sso-configure-api)
    - [applicationTemplate](/graph/api/resources/applicationtemplate)
    - [application](/graph/api/resources/application)
    - [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy)
    - [servicePrincipal](/graph/api/resources/serviceprincipal)

## <a name="next-steps"></a>Próximas etapas

- Experimente a API do Microsoft Graph no[Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer). 
- Saiba mais sobre como adicionar autenticação e autorização aos aplicativos Web e às APIs da Web usando [estes exemplos](/azure/active-directory/develop/sample-v2-code).
