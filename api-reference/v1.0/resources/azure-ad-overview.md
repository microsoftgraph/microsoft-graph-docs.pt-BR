---
title: Trabalhar com os recursos do Azure Active Directory no Microsoft Graph
description: 'Com o Microsoft Graph, você pode acessar recursos do Azure Active Directory (Azure AD) para habilitar cenários como gerenciar funções de administrador (diretório), convidando usuários externos para uma organização e, se você for um Provedor de Solução na Nuvem (CSP), gerenciar dados do cliente. O Microsoft Graph também fornece métodos que os aplicativos podem usar para, por exemplo, descobrir informações sobre grupo transitivo e associações de função de usuário. '
localization_priority: Priority
author: dkershaw10
ms.prod: identity-and-access
doc_type: conceptualPageType
ms.openlocfilehash: 46ec3aa87714b48570f529764e64e848189e75d8
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118425"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Trabalhar com os recursos do Azure Active Directory no Microsoft Graph

Com o Microsoft Graph, você pode acessar recursos do [Azure Active Directory (Azure AD)](/azure/active-directory/active-directory-whatis) para habilitar cenários como gerenciar funções de administrador (diretório), convidando usuários externos para uma organização e, se você for um [Provedor de Solução na Nuvem (CSP)](https://partner.microsoft.com/cloud-solution-provider), gerenciar dados do cliente. O Microsoft Graph também fornece métodos que os aplicativos podem usar para, por exemplo, descobrir informações sobre grupo transitivo e associações de função de usuário.

> **Observação**: alguns recursos do Azure AD são documentados em outras seções da API de referência. Para saber mais, confira [Usuários](users.md) e [Grupos](group.md).


## <a name="authorization"></a>Autorização

Para chamar as APIs do Microsoft Graph nos recursos do Azure AD, seu aplicativo precisará das permissões adequadas. Muitas das APIs expostas nos recursos do Azure AD exigem uma das [permissões de _diretório_](/graph/permissions-reference#directory-permissions). As permissões de diretório são altamente privilegiadas e sempre exigem o consentimento do administrador.

Se seu aplicativo estiver agindo em nome de um usuário (permissões delegadas), é provável que esse usuário precise ser um membro de uma [função de administrador](/azure/active-directory/active-directory-assign-admin-roles) apropriada para que seu aplicativo chame com êxito muitas das APIs do Azure AD.

Para saber mais sobre permissões, incluindo permissões delegadas e de aplicativos, confira o artigo sobre [Permissões](/graph/permissions-reference).

## <a name="common-use-cases"></a>Casos comuns de uso

A tabela a seguir lista alguns casos comuns de uso de recursos do Azure AD.

| **Casos de uso**        | **Recursos REST** | **Confira também** |
|:---------------|:--------|:----------|
| **Métodos e objeto de diretório** | | |
| `directoryObject` é a classe-base da qual herdam muitos recursos de diretório, como usuários e grupos. O Microsoft Graph expõe vários métodos que você pode usar para descobrir informações sobre usuários, grupos e outros objetos de diretório. Por exemplo, é possível verificar a associação transitiva em uma lista de grupos, retornar todos os grupos e funções de diretório da qual um objeto de diretório é membro transitivo ou obter todos os recursos de um tipo especificado (como o usuário ou grupo) de uma lista de IDs de recurso genérico. | [directoryObject](../resources/directoryobject.md) | N/D |
| **Gerenciar funções de diretório (administrador)** | | |
| Ativar funções de diretório em um locatário do Azure AD e gerenciar associações de usuário em funções de diretório. As funções de diretório também são conhecidas como funções de administrador. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) | [Atribuindo funções de administrador no Azure Active Directory](/azure/active-directory/active-directory-assign-admin-roles) |
| Aplica configurações de grupo predefinidas a um locatário ou a instâncias de recurso individuais. Configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nome de exibições de grupo, se os usuários convidados podem ser proprietários de grupo e muito mais. | [groupSetting](../resources/groupsetting.md) <br/>[groupSettingTemplate](../resources/groupsettingtemplate.md)| [Cmdlets Azure Active Directory para definição de configurações de grupo](/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| **Gerenciar dispositivos** | | |
| Gerenciar os dispositivos registrados na organização. Os dispositivos são registrados a usuários e incluem itens como laptops, computadores desktop e celulares. Os dispositivos são em geral criados na nuvem usando o Serviço de Registro de Dispositivo ou por meio do Microsoft Intune. Eles são utilizados por políticas de acesso condicional para a autenticação multifator. | [device](../resources/device.md) | [Introdução ao registro de dispositivos do Azure Active Directory](/azure/active-directory/active-directory-device-registration-overview).<br/><br/>[O que é o InTune?](/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Registrar dispositivos para o gerenciamento no Intune](/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **Gerenciamento de locatário do parceiro** | | |
| Obter informações sobre parcerias com locatários do cliente.<br/><br/>**Observação:** Isso se aplica somente a locatários do parceiro. Os locatários do parceiro são locatários do Azure AD que pertencem a parceiros da Microsoft que fazem parte do [Provedor de Soluções na Nuvem da Microsoft](https://partnercenter.microsoft.com/partner/programs), Syndication do Office 365 ou de programas de parceiro de Consultor Microsoft. | [contract](../resources/contract.md) | [Chamar o Microsoft Graph por um aplicativo de Provedor de Soluções em Nuvem](/graph/auth-cloudsolutionprovider) |
| Gerenciar os domínios associados a um locatário. As operações de domínio permitem que os registradores automatizem a associação de domínio para serviços como o Microsoft 365. | [domain](../resources/domain.md) | [Adicionar um nome de domínio personalizado ao Azure Active Directory](/azure/active-directory/active-directory-domains-add-azure-portal) |
| **Gerenciamento de locatário** | | |
| Obter informações sobre uma organização, como seu endereço comercial, contatos de notificação e técnicos, os planos de serviço em que está inscrita em e os domínios associados a ela. | [organization](../resources/organization.md) | N/D |
| Obter informações sobre SKUs do serviço nos quais a empresa está inscrita. | [subscribedSku](../resources/subscribedsku.md) | N/D |
| Convidar usuários externos (convidado) para uma organização. | [invitation](../resources/invitation.md) | [O que é a colaboração B2B do Azure AD?](/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b) |
| Gerenciar a identidade visual da experiência de entrada de uma organização. | [organizationalbranding](../resources/organizationalbrandingproperties.md) | [Adicionar identidade visual à página de entrada do Azure Active Directory da sua organização](/azure/active-directory/fundamentals/customize-branding)|
| **Solicitações de consentimento** | | |
| Gerenciar o fluxo de trabalho da solicitação de consentimento para usuários que tentam acessar aplicativos que requerem autorização do administrador.  | [API de solicitações de consentimento](../resources/consentrequests-root.md) |[Configure o fluxo de trabalho de consentimento do administrador](/azure/active-directory/manage-apps/configure-admin-consent-workflow) |

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas
APIs e recursos de diretório podem criar novas maneiras para você relacionar-se com os usuários e gerenciar as experiências deles com o Microsoft Graph. Para saber mais:

- Examine os métodos e as propriedades dos recursos mais úteis para o seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/partners).
