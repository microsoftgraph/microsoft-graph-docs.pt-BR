---
title: Trabalhar com os recursos do Azure Active Directory no Microsoft Graph
description: O Microsoft Graph para o Azure AD (Azure Active Directory) fornece as APIs REST para ajudá-lo a gerenciar a organização, os recursos e os ativos.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: identity-access
author: dkershaw10
ms.openlocfilehash: 689ae5e1c4c3c13dff1ae6d5443e8a8b22e3039f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133382"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Trabalhar com os recursos do Azure Active Directory no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Com o Microsoft Graph, você pode acessar recursos do [Azure Active Directory (Azure AD)](/azure/active-directory/active-directory-whatis) para habilitar cenários como gerenciar funções de administrador (diretório), convidando usuários externos para uma organização e, se você for um [Provedor de Solução na Nuvem (CSP)](https://partner.microsoft.com/cloud-solution-provider), gerenciar dados do cliente. O Microsoft Graph também fornece métodos que os aplicativos podem usar, por exemplo, para descobrir informações sobre grupo transitivo e associações de função de usuário.

> **Observação**: alguns recursos do Azure AD são documentados em outras seções da API de referência. Para saber mais, confira [Usuários](users.md) e [Grupos](group.md).


## <a name="authorization"></a>Autorização

Para chamar as APIs do Microsoft Graph nos recursos do Azure AD, seu aplicativo precisará das permissões adequadas. Muitas das APIs expostas nos recursos do Azure AD exigem uma das [permissões de _diretório_](/graph/permissions-reference#directory-permissions). As permissões de diretório são altamente privilegiadas e sempre exigem o consentimento do administrador.

Se seu aplicativo estiver agindo em nome de um usuário (permissões delegadas), é provável que esse usuário precise ser um membro de uma [função de administrador](/azure/active-directory/active-directory-assign-admin-roles) apropriada para que seu aplicativo chame com êxito muitas das APIs do Azure AD.

Para saber mais sobre permissões, incluindo permissões delegadas e de aplicativos, confira o artigo sobre [Permissões](/graph/permissions-reference).

## <a name="common-use-cases"></a>Casos comuns de uso

A tabela a seguir lista alguns casos comuns de uso de recursos do Azure AD.

| **Casos de uso**        | **Recursos REST** | **Confira também** |
|:-----------------|:--------|:----------|
| **Métodos e objeto de diretório** | | |
| `directoryObject` é a classe-base da qual herdam muitos recursos de diretório, como usuários e grupos. O Microsoft Graph expõe vários métodos que você pode usar para descobrir informações sobre usuários, grupos e outros objetos de diretório. Por exemplo, é possível verificar a associação transitiva em uma lista de grupos, retornar todos os grupos e funções de diretório da qual um objeto de diretório é membro transitivo ou obter todos os recursos de um tipo especificado (como o usuário ou grupo) de uma lista de IDs de recurso genérico. | [directoryObject](../resources/directoryobject.md) | N/D |
| **Gerenciar funções de diretório (administrador), unidades administrativas, configurações de diretório e política** | | |
| Ative funções de diretório em um locatário do Azure AD e gerencie associações de usuário em funções de diretório. As funções de diretório também são conhecidas como funções de administrador. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles)|
| Gerencie unidades administrativas. As funções de diretório delegam autoridade em todos os locatários aos seus membros. Um administrador pode criar e gerenciar unidades administrativas para delegar a autoridade administrativa com escopo de maior granularidade para os usuários. | [administrativeUnit](../resources/administrativeunit.md) | [Gerenciamento de unidades administrativas no Azure AD](/azure/active-directory/active-directory-administrative-units-management) |
| Aplique configurações de diretórios predefinidas a um locatário ou a instâncias de recurso individuais. Atualmente, apenas as configurações para grupos do Microsoft 365 são compatíveis. Aplica configurações de grupo predefinidas a um locatário ou a instâncias de recurso individuais. Configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nome de exibições de grupo, se os usuários convidados podem ser proprietários de grupo e muito mais. | [directorySetting](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [Cmdlets do Azure Active Directory para definição de configurações de grupo](/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| Aplique políticas do Azure AD para aplicativos, entidades de serviço, grupos ou toda a organização. As políticas para mapeamento de declarações, emissão de token, duração de token, descoberta de realm inicial e mais são suportados.  | [Políticas disponíveis](../resources/policy-overview.md) | Não disponível |
| **Acesso seguro privilegiado ao Azure AD** | | |
| Gerencie e monitore o acesso privilegiado com limite de tempo aos diretório e os recursos do Azure para administradores e profissionais de TI com PIM (Privileged Identity Management). | [APIs de Privileged Identity Management](../resources/privilegedidentitymanagement-root.md) | [O que é o Azure AD Privileged Identity Management?](/azure/active-directory/active-directory-privileged-identity-management-configure)|
| Monitore os eventos de risco de identidade, como os usuários fazendo logon em dispositivos infectado por malware ou locais desconhecidos. | [API do serviço de proteção de identidade](../resources/identityprotection-root.md) | [Azure Active Directory Identity Protection](/azure/active-directory/active-directory-identityprotection)<br/><br/>[Eventos de risco do Azure Active Directory](/azure/active-directory/active-directory-reporting-risk-events) |
| **Gerenciar dispositivos** | | |
| Gerenciar os dispositivos registrados na organização. Os dispositivos são registrados a usuários e incluem itens como laptops, computadores desktop e celulares. Os dispositivos são em geral criados na nuvem usando o Serviço de Registro de Dispositivo ou por meio do Microsoft Intune. Eles são utilizados por políticas de acesso condicional para a autenticação multifator. | [device](../resources/device.md) | [Introdução ao registro de dispositivos do Azure Active Directory](/azure/active-directory/active-directory-device-registration-overview) |
| **Gerenciamento de aplicativos** | | |
| Gerencie a configuração do aplicativo em um locatário do desenvolvedor. | [application](../resources/application.md) | [Aplicativo e objetos de entidade de serviço no Azure Active Directory](/azure/active-directory/develop/active-directory-application-objects) |
| Gerencie aplicativos instalados em um locatário. | [servicePrinicpal](../resources/serviceprincipal.md) | [Aplicativo e objetos de entidade de serviço no Azure Active Directory](/azure/active-directory/develop/active-directory-application-objects) |
| Gerencie as permissões consentidas por usuários e administradores em aplicativos instalados em um locatário. | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | N/D |
| Gerencie usuários, grupos e associações de função da entidade de serviço em aplicativos instalados em um locatário. | [appRoleAssignment](../resources/approleassignment.md) | N/D |
| **Gerenciamento de locatário do parceiro** | | |
| Obter informações sobre parcerias com locatários do cliente. <br/><br/>**Observação:** Isso se aplica somente a locatários do parceiro. Os locatários do parceiro são locatários do Azure AD que pertencem a parceiros da Microsoft que fazem parte do [Provedor de Soluções na Nuvem da Microsoft](https://partnercenter.microsoft.com/partner/programs), Syndication do Office 365 ou de programas de parceiro de Consultor Microsoft.| [contract](../resources/contract.md) | [Chamar o Microsoft Graph por um aplicativo de Provedor de Soluções em Nuvem](/graph/auth-cloudsolutionprovider) |
| Gerenciar os domínios associados a um locatário. As operações de domínio permitem que os registradores automatizem a associação de domínio para serviços como o Microsoft 365. | [domain](../resources/domain.md) | [Adicionar um nome de domínio personalizado ao Azure Active Directory](/azure/active-directory/active-directory-domains-add-azure-portal) |
| **Gerenciamento de locatário** | | |
| Obter informações sobre uma organização, como seu endereço comercial, contatos de notificação e técnicos, os planos de serviço em que está inscrita em e os domínios associados a ela. | [organization](../resources/organization.md) | N/D |
| Obter informações sobre SKUs do serviço nos quais a empresa está inscrita. | [subscribedSku](../resources/subscribedsku.md) | N/D |
| Convidar usuários externos (convidado) para uma organização. | [invitation](../resources/invitation.md) | [O que é a colaboração B2B do Azure AD?](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| Gerenciar a identidade visual da experiência de entrada de uma organização. | [organizationalbranding](../resources/organizationalbrandingproperties.md) | [Adicionar identidade visual à página de entrada do Azure Active Directory da sua organização](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding)|
| **Avaliações do Access** | | |
| Certifique-se de que as associações ao grupo e os direitos de acesso ao aplicativo estejam corretos com as análises de acesso. | [API de revisões de acesso](../resources/accessreviews-root.md) |[Revisões de acesso ao Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas
APIs e recursos de diretório podem criar novas maneiras para você relacionar-se com os usuários e gerenciar as experiências deles com o Microsoft Graph. Para saber mais:

- Examine os métodos e as propriedades dos recursos mais úteis para o seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).
