---
title: Visão geral da API de gerenciamento de identidade e acesso do Azure AD
description: 'O Active Directory do Azure (Azure AD) ajuda a centralizar o gerenciamento de identidade e acesso para permitir acesso seguro e produtivo entre aplicativos, dispositivos, serviços e infraestrutura. As organizações podem usar o Azure AD para gerenciar identidades e controlar o acesso em ambientes locais, híbridos e em nuvem.  '
author: jackson-woods
localization_priority: Priority
ms.prod: identity-access
ms.custom: scenarios:getting-started
ms.openlocfilehash: a2ea9b042119c110d4063c19877b9d4b7694423a
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761441"
---
# <a name="azure-ad-identity-and-access-management-api-overview"></a>Visão geral da API de gerenciamento de identidade e acesso do Azure AD

O Active Directory do Azure (Azure AD) ajuda a centralizar o gerenciamento de identidade e acesso para permitir acesso seguro e produtivo entre aplicativos, dispositivos, serviços e infraestrutura. As organizações podem usar o Azure AD para gerenciar identidades e controlar o acesso em ambientes locais, híbridos e em nuvem.

Você pode usar as APIs REST do Azure AD no Microsoft Graph para criar fluxos de trabalho exclusivos entre os [recursos](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0) do Azure AD e serviços de terceiros.

## <a name="why-use-the-azure-ad-apis"></a>Por que usar as APIs do Azure AD?

Mais de 15 milhões de organizações usam o Azure AD ao se inscreverem em serviços em nuvem da Microsoft, como o Microsoft 365, Microsoft Azure, Enterprise Mobility Suite ou Microsoft 365.

Os desenvolvedores corporativos usam o Microsoft Graph para integrar o gerenciamento de identidades do Azure AD e outros serviços para automatizar fluxos de trabalho administrativos, como a integração (e rescisão) de funcionários, a manutenção de perfis, a implantação de licenças e muito mais.

Para muitos desenvolvedores corporativos, o Microsoft Graph e o Azure AD ajudam a "elevar e deslocar" os aplicativos existentes para a nuvem, acelerando a transformação digital de uma organização. Você pode aproveitar os recursos do Azure AD para adicionar mecanismos de controle de acesso a aplicativos, incluindo a verificação de associação de grupo, a função de diretório ou a associação de unidades administrativas de um usuário.

Você pode usar o Microsoft Graph e o Azure AD como uma maneira rápida e fácil de alcançar mais de 15 milhões de organizações, incluindo 90% das empresas da Fortune 500 que já usam os serviços do Azure AD. Os aplicativos integrados apresentam experiências de logon sem interrupções e podem usar dados organizacionais existentes para criar experiências personalizadas.

Você pode usar as APIs do Azure AD no Microsoft Graph para consultar o perfil do usuário, encontrar outros usuários, gerenciar relações organizacionais, rastrear atribuições ou criar soluções originais que incorporem dados organizacionais existentes. Essas APIs fornecem uma base sólida para integrar aplicativos de negócios personalizados aos serviços digitais existentes de uma organização.

### <a name="access-users-and-groups"></a>Acessar usuários e grupos

Você pode usar as APIs do Azure AD no Microsoft Graph para:

- Pesquisar e gerenciar informações de [perfil de usuário](/graph/api/resources/user?view=graph-rest-1.0), como nome, foto, endereço de email, cargo, localização do escritório e muito mais de usuários na sua organização.
- Criar [grupos](/graph/api/resources/groups-overview?view=graph-rest-1.0) para projetos e equipes na sua organização. Adicionar e remover membros do grupo para controlar o acesso aos recursos. (Os grupos dinâmicos podem alterar automaticamente a associação com base nos valores da propriedade do usuário).
- Para controlar o acesso, você pode verificar a [associação transitiva](/graph/api/user-checkmembergroups?view=graph-rest-1.0) em uma lista de grupos ou obter todos os recursos de um tipo especificado (como um usuário ou grupo) de uma lista de [IDs de recursos genéricos](/graph/api/directoryobject-getbyids?view=graph-rest-1.0).

### <a name="manage-directory-roles"></a>Gerenciar funções de diretório

Você pode atribuir usuários a [funções de diretório](/graph/api/resources/directoryrole?view=graph-rest-1.0) administrativas predefinidas do Azure AD, que concede permissão para executar tarefas específicas.

### <a name="manage-devices"></a>Gerenciar dispositivos

[Gerencie os dispositivos](/azure/active-directory/device-management-introduction) registrados na organização. Os dispositivos são registrados a usuários e incluem itens como laptops, computadores desktop e celulares. Os dispositivos são em geral criados na nuvem usando o Serviço de Registro de Dispositivo ou por meio do Microsoft Intune. Eles são utilizados por políticas de acesso condicional para a autenticação multifator.

### <a name="partner-tenant-management"></a>Gerenciamento de locatário do parceiro

Os parceiros da Microsoft que revendem e gerenciam o Microsoft Online Services (como o Microsoft 365, o Microsoft Azure e o CRM Online) podem exibir os [locatários da organização](/graph/api/resources/contract?view=graph-rest-1.0) que gerenciam atualmente.

Você também pode [gerenciar domínios](/graph/api/resources/domain?view=graph-rest-1.0) associados a um locatário. As operações de domínio permitem que os parceiros da Microsoft automatizem o registro de domínio para serviços, como o Microsoft 365.

### <a name="tenant-management"></a>Gerenciamento de locatários

As APIs do Azure AD para o gerenciamento de locatários permitem:

- Obter informações sobre uma [organização](/graph/api/resources/organization?view=graph-rest-1.0), como seu endereço comercial, contatos de notificação e técnicos, assinaturas de serviço ativas e os domínios associados a ela.
- Obter informações sobre [SKUs do serviço](/graph/api/resources/subscribedsku?view=graph-rest-1.0) nos quais a empresa está inscrita.
- [Convidar usuários externos](/graph/api/resources/invitation?view=graph-rest-1.0) (convidados) para uma organização.

### <a name="monitor-identity-risks-preview"></a>Monitorar os riscos de identidade (prévia)

A maioria das violações de segurança resulta de invasores que roubam a identidade do usuário. Os invasores tem sido muito eficientes em aproveitar de violações de terceiros, ataques de pulverização de senhas e ataques de phishing sofisticados. Isso significa que você precisa proteger todas as suas contas de usuário desses ataques e proativamente evitar identidades comprometidas de serem violadas.

O Azure AD usa algoritmos de aprendizado de máquina adaptativos e heurística para detectar anomalias que indicam potencialmente contas comprometidas. Com esses dados, o Azure Active Directory Identity Protection protege os usuários com políticas de acesso condicional baseadas em risco e gera relatórios e alertas com base em suas detecções.

Hoje, o Microsoft Graph oferece acesso fácil aos clientes do Azure AD Premium P2 para [consultar eventos de risco detectados pelo Identity Protection](/graph/api/resources/identityprotection-root?view=graph-rest-beta), incluindo o tipo do evento de risco, a gravidade, a data, a hora, o local, o usuário afetado e mais. Os clientes podem então usar esses eventos em sistemas SIEM e aplicativos de segurança.

### <a name="activate-users-into-privileged-roles-preview"></a>Ativar usuários em funções privilegiadas (prévia)

Você pode garantir o acesso a recursos ativando privilégios administrativos sob demanda. O [Gerenciamento de Identidade Privilegiada](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) é oferecido no Azure AD Premium P2.

### <a name="manage-user-access-reviews-preview"></a>Gerenciar as revisões de acesso do usuário (prévia)

Você pode configurar revisões de acesso de associações a grupos e acesso a aplicativos. As [Revisões de Acesso](/graph/api/resources/accessreviews-root?view=graph-rest-beta) são apresentadas no Azure AD Premium P2.

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [API de gerenciamento de acesso e identidade do Azure AD no Microsoft Graph v1.0](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0)
- [API de gerenciamento de acesso e identidade do Azure AD no Microsoft Graph beta](/graph/api/resources/azure-ad-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

- Saiba como [Usar as APIs REST do Azure AD](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0).
- Use o Azure AD para se [autenticar](./auth/index.yml) no Microsoft Graph.
- Integre o [logon do Azure AD](https://azure.microsoft.com/develop/identity/signin/) ao seu aplicativo ou website.
- Confira o [Changelog](changelog.md) para obter informações sobre novidades nas APIs do Azure AD.
- Explore [exemplos](https://developer.microsoft.com/graph/graph/examples) para obter mais ideias sobre como usar o Microsoft Graph.