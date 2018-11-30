---
title: Trabalhar com os recursos do Azure Active Directory no Microsoft Graph
description: 'Com o Microsoft Graph, você pode acessar recursos do Windows Azure Active Directory (AD Azure) para habilitar cenários, como gerenciar funções de administrador (diretório), convidar usuários externos a uma organização e, se você for um provedor de solução de nuvem (CSP), gerenciar sua dados do cliente. O Microsoft Graph também fornece métodos apps podem usar, por exemplo, para descobrir informações sobre associações de grupo e função da transitivas dos usuários. '
ms.openlocfilehash: 4f33004e5bacf71c2e7cd3af5bad78448983dec7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041029"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Trabalhar com os recursos do Azure Active Directory no Microsoft Graph

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Com o Microsoft Graph, você pode acessar recursos do [Windows Azure Active Directory (AD Azure)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis) para habilitar cenários, como gerenciar funções de administrador (diretório), convidar usuários externos para uma organização, e, se você for um [Provedor de solução da nuvem (CSP)](https://partner.microsoft.com/cloud-solution-provider), Gerenciando dados do seu cliente. O Microsoft Graph também fornece métodos apps podem usar, por exemplo, para descobrir informações sobre associações de grupo e função da transitivas dos usuários. 

> **Observação**: alguns recursos do Azure AD são documentados em outras seções da API de referência. Para saber mais, confira os artigos sobre [Usuários](users.md) e [Grupos](group.md).


## <a name="authorization"></a>Autorização
 
Para chamar as APIs do Microsoft Graph nos recursos do Azure AD, seu aplicativo precisará das permissões adequadas. Muitas das APIs expostas nos recursos do Azure AD exigem uma das [permissões de _diretório_](/graph/permissions-reference#directory-permissions). As permissões de diretório são altamente privilegiadas e sempre exigem o consentimento do administrador. 

Se seu aplicativo estiver agindo em nome de um usuário (permissões delegadas), é provável que esse usuário precise ser um membro de uma [função de administrador](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles) apropriada para que seu aplicativo chame com êxito muitas das APIs do Azure AD.

Para saber mais sobre permissões, incluindo permissões delegadas e de aplicativos, confira o artigo sobre [Permissões](/graph/permissions-reference). 

## <a name="common-use-cases"></a>Casos comuns de uso 

A tabela a seguir lista alguns casos comuns de uso de recursos do Azure AD.

| **Casos de uso**        | **Recursos REST** | **Confira também** |
|:-----------------|:--------|:----------|
| **Métodos e objeto de diretório** | | |
| `directoryObject` é a classe-base da qual herdam muitos recursos de diretório, como usuários e grupos. O Microsoft Graph expõe vários métodos que você pode usar para descobrir informações sobre usuários, grupos e outros objetos de diretório. Por exemplo, é possível verificar a associação transitiva em uma lista de grupos, retornar todos os grupos e funções de diretório da qual um objeto de diretório é membro transitivo ou obter todos os recursos de um tipo especificado (como o usuário ou grupo) de uma lista de IDs de recurso genérico. | [directoryObject](../resources/directoryobject.md) | N/D |
| **Gerenciar funções de diretório (administrador), unidades administrativas, configurações de diretório e política** | | |
| Ativar funções de diretório em um locatário do Azure AD e gerenciar associações de usuário em funções de diretório. As funções de diretório também são conhecidas como funções de administrador. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[Atribuindo funções de administrador no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)|
| Gerencie unidades administrativas. Funções de diretório delegam autoridade todo o locatário seus membros. Um administrador pode criar e gerenciar unidades administrativas para delegar a forma mais granular com escopo autoridade administrativa aos usuários. | [administrativeUnit](../resources/administrativeunit.md) | [Gerenciamento de unidades administrativas no Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-administrative-units-management) |
| Aplica configurações de diretório predefinidos em um locatário ou para instâncias de recursos individuais. Atualmente, somente as configurações para o Office 365 grupos são suportadas. Comportamentos de controle de configurações de diretório, como listas de palavras bloqueados para nomes de grupo de exibição, se os usuários de convidado poderão ser proprietários do grupo e muito mais. | [directorySetting](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [Cmdlets Azure Active Directory para definição de configurações de grupo](https://docs.microsoft.com/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| Aplica políticas de Azure AD para aplicativos, entidades de serviço, grupos ou toda a organização. Atualmente, há suporte para políticas de vida útil do token e descoberta de realm inicial.  | [política](../resources/policy.md) | N/D |
| **Acesso privilegiado seguro para o Windows Azure AD** | | |
| Gerenciar e monitorar o limite de tempo de acesso privilegiado de diretório e recursos do Windows Azure para administradores e profissionais de TI com o gerenciamento de identidade privilegiado (PIM). | [API de gerenciamento de identidade privilegiado](../resources/privilegedidentitymanagement-root.md) | [O que é gerenciamento de identidade do Azure AD privilegiado?](https://docs.microsoft.com/azure/active-directory/active-directory-privileged-identity-management-configure)|
| Monitorar eventos de risco de identidade, como usuários entrando a partir de dispositivos infectados por malware ou familiarizados locais. | [API do serviço de proteção de identidade](../resources/identityprotection-root.md) | [Proteção de identidade do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-identityprotection)<br/><br/>[Eventos de risco do Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events) |
| **Gerenciar dispositivos** | | |
| Gerenciar os dispositivos registrados na organização. Os dispositivos são registrados a usuários e incluem itens como laptops, computadores desktop e celulares. Os dispositivos são em geral criados na nuvem usando o Serviço de Registro de Dispositivo ou por meio do Microsoft Intune. Eles são utilizados por políticas de acesso condicional para a autenticação multifator. | [device](../resources/device.md) | [Introdução ao registro de dispositivos do Windows Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview)<br/><br/>[O que é o InTune?](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Registrar dispositivos para o gerenciamento no Intune](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **Gerenciamento de aplicativo** | | |
| Gerencie a configuração de aplicativos em um locatário de desenvolvedor. | [application](../resources/application.md) | [Aplicativo e objetos de entidade de serviço no Windows Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Gerencie os aplicativos instalados em um locatário. | [servicePrinicpal](../resources/serviceprincipal.md) | [Aplicativo e objetos de entidade de serviço no Windows Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Gerenciar permissões consentiu pelos usuários e administradores nos aplicativos instalados em um locatário. | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | N/D |
| Gerencie usuários, grupos e associações de função principal de serviço nos aplicativos instalados em um locatário. | [appRoleAssignment](../resources/approleassignment.md) | N/D |
| **Gerenciamento de locatário do parceiro** | | |
| Obter informações sobre parcerias com locatários do cliente. <br/><br/>**Observação:** Isso se aplica somente a locatários do parceiro. Os locatários do parceiro são locatários do Azure AD que pertencem a parceiros da Microsoft que fazem parte do [Provedor de Soluções na Nuvem da Microsoft](https://partnercenter.microsoft.com/partner/programs), Syndication do Office 365 ou de programas de parceiro de Consultor Microsoft.| [contract](../resources/contract.md) | [Chamar o Microsoft Graph por um aplicativo de Provedor de Soluções em Nuvem](/graph/auth-cloudsolutionprovider) |
| Gerenciar os domínios associados a um locatário. As operações de domínio permitem que os registradores automatizem a associação de domínio para serviços como o Office 365. | [domain](../resources/domain.md) | [Adicionar um nome de domínio personalizado ao Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal) |
| **Gerenciamento de locatário** | | |
| Obter informações sobre uma organização, como seu endereço comercial, contatos de notificação e técnicos, os planos de serviço em que está inscrita em e os domínios associados a ela. | [organization](../resources/organization.md) | N/D |
| Obter informações sobre SKUs do serviço nos quais a empresa está inscrita. | [subscribedSku](../resources/subscribedsku.md) | N/D |
| Convidar usuários externos (convidado) para uma organização. | [invitation](../resources/invitation.md) | [O que é a colaboração B2B do Azure AD?](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| **Avaliações de acesso** | | |
| Certifique-se de associações de grupo e direitos de acesso do aplicativo estão corretos com as revisões de acesso | [Access analisa API](../resources/accessreviews-root.md) |[Analisa de acesso do Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |
## <a name="next-steps"></a>Próximas etapas
APIs e recursos de diretório podem criar novas maneiras para você relacionar-se com os usuários e gerenciar as experiências deles com o Microsoft Graph. Para saber mais: 

- Examine os métodos e as propriedades dos recursos mais úteis para o seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

