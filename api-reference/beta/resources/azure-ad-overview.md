---
title: Trabalhar com os recursos do Azure Active Directory no Microsoft Graph
description: O Microsoft Graph para o Azure AD (Azure Active Directory) fornece as APIs REST para ajudá-lo a gerenciar a organização, os recursos e os ativos.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b2d6bff52e7defbf487b0cbe9016dd278591588b
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080867"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Trabalhar com os recursos do Azure Active Directory no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Com o Microsoft Graph, você pode acessar recursos do [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis) para habilitar cenários como gerenciar funções de administrador (diretório), convidando usuários externos para uma organização e, se você for um [Provedor de Solução na Nuvem (CSP)](https://partner.microsoft.com/cloud-solution-provider), gerenciar dados do cliente. O Microsoft Graph também fornece métodos que os aplicativos podem usar, por exemplo, para descobrir informações sobre grupo transitivo e associações de função de usuário.

> **Note**: Some Azure AD resources are documented in other sections of the API reference. For more information, see [Users](users.md) and [Groups](group.md).


## <a name="authorization"></a>Autorização

To call the Microsoft Graph APIs on Azure AD resources, your app will need the appropriate permissions. Many of the APIs exposed on Azure AD resources require one of the [_Directory_ permissions](/graph/permissions-reference#directory-permissions). Directory permissions are highly privileged and always require administrator consent.

Se seu aplicativo estiver agindo em nome de um usuário (permissões delegadas), é provável que esse usuário precise ser um membro de uma [função de administrador](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles) apropriada para que seu aplicativo chame com êxito muitas das APIs do Azure AD.

Para saber mais sobre permissões, incluindo permissões delegadas e de aplicativos, confira o artigo sobre [Permissões](/graph/permissions-reference).

## <a name="common-use-cases"></a>Casos comuns de uso

A tabela a seguir lista alguns casos comuns de uso de recursos do Azure AD.

| **Casos de uso**        | **Recursos REST** | **Confira também** |
|:-----------------|:--------|:----------|
| **Métodos e objeto de diretório** | | |
| `directoryObject` is the base class that many directory resources, like users and groups, inherit from. Microsoft Graph exposes several methods that you can use to discover information about users, groups, and other directory objects. For example, you can check for transitive membership in a list of groups, return all the groups and directory roles that a directory object is a transitive member of, or get all the resources of a specified type (like user or group) from a list of generic resource IDs. | [directoryObject](../resources/directoryobject.md) | N/D |
| **Gerenciar funções de diretório (administrador), unidades administrativas, configurações de diretório e política** | | |
| Activate directory roles in an Azure AD tenant and manage user memberships in directory roles. Directory roles are also known as administrator roles. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[Atribuindo funções de administrador no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)|
| Gerencie unidades administrativas. As funções de diretório delegam autoridade em todos os locatários aos seus membros. Um administrador pode criar e gerenciar unidades administrativas para delegar a autoridade administrativa com escopo de maior granularidade para os usuários. | [administrativeUnit](../resources/administrativeunit.md) | [Gerenciamento de unidades administrativas no Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-administrative-units-management) |
| Aplique configurações de diretórios predefinidas a um locatário ou a instâncias de recurso individuais. Atualmente, apenas as configurações para grupos do Microsoft 365 são compatíveis. Aplica configurações de grupo predefinidas a um locatário ou a instâncias de recurso individuais. Configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nome de exibições de grupo, se os usuários convidados podem ser proprietários de grupo e muito mais. | [directorySetting](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [Cmdlets do Azure Active Directory para definição de configurações de grupo](https://docs.microsoft.com/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| Aplique políticas do Azure AD para aplicativos, entidades de serviço, grupos ou toda a organização. As políticas para mapeamento de declarações, emissão de token, duração de token, descoberta de realm inicial e mais são suportados.  | [Políticas disponíveis](../resources/policy-overview.md) | N/A |
| **Acesso seguro privilegiado ao Azure AD** | | |
| Gerencie e monitore o acesso privilegiado com limite de tempo aos diretório e os recursos do Azure para administradores e profissionais de TI com PIM (Privileged Identity Management). | [APIs de Privileged Identity Management](../resources/privilegedidentitymanagement-root.md) | [O que é o Azure AD Privileged Identity Management?](https://docs.microsoft.com/azure/active-directory/active-directory-privileged-identity-management-configure)|
| Monitore os eventos de risco de identidade, como os usuários fazendo logon em dispositivos infectado por malware ou locais desconhecidos. | [API do serviço de proteção de identidade](../resources/identityprotection-root.md) | [Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/active-directory-identityprotection)<br/><br/>[Eventos de risco do Azure Active Directory](/azure/active-directory/active-directory-reporting-risk-events) |
| **Gerenciar dispositivos** | | |
| Manage devices registered in the organization. Devices are registered to users and include items like laptops, desktops, tablets, and mobile phones. Devices are typically created in the cloud using the Device Registration Service or by Microsoft Intune. They're used by conditional access policies for multifactor authentication. | [device](../resources/device.md) | [Introdução ao registro de dispositivos do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview)<br/><br/>[O que é o InTune?](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Registrar dispositivos para o gerenciamento no Intune](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **Gerenciamento de aplicativos** | | |
| Gerencie a configuração do aplicativo em um locatário do desenvolvedor. | [application](../resources/application.md) | [Aplicativo e objetos de entidade de serviço no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Gerencie aplicativos instalados em um locatário. | [servicePrinicpal](../resources/serviceprincipal.md) | [Aplicativo e objetos de entidade de serviço no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Gerencie as permissões consentidas por usuários e administradores em aplicativos instalados em um locatário. | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | N/D |
| Gerencie usuários, grupos e associações de função da entidade de serviço em aplicativos instalados em um locatário. | [appRoleAssignment](../resources/approleassignment.md) | N/D |
| **Gerenciamento de locatário do parceiro** | | |
| Obter informações sobre parcerias com locatários do cliente. <br/><br/>**Note:** This applies to partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of the [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.| [contract](../resources/contract.md) | [Chamar o Microsoft Graph por um aplicativo de Provedor de Soluções em Nuvem](/graph/auth-cloudsolutionprovider) |
| Manage domains associated with a tenant. Domain operations enable registrars to automate domain association for services such as Microsoft 365. | [domain](../resources/domain.md) | [Adicionar um nome de domínio personalizado ao Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal) |
| **Gerenciamento de locatário** | | |
| Obter informações sobre uma organização, como seu endereço comercial, contatos de notificação e técnicos, os planos de serviço em que está inscrita em e os domínios associados a ela. | [organization](../resources/organization.md) | N/D |
| Obter informações sobre SKUs do serviço nos quais a empresa está inscrita. | [subscribedSku](../resources/subscribedsku.md) | N/D |
| Convidar usuários externos (convidado) para uma organização. | [invitation](../resources/invitation.md) | [O que é a colaboração B2B do Azure AD?](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| **Avaliações do Access** | | |
| Certifique-se que as associações ao grupo e os direitos de acesso ao aplicativo estão corretos com as revisões de acesso | [API de revisões de acesso](../resources/accessreviews-root.md) |[Revisões de acesso ao Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas
Directory resources and APIs can open up new ways for you to engage with users and manage their experiences with Microsoft Graph. To learn more:

- Examine os métodos e as propriedades dos recursos mais úteis para o seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

