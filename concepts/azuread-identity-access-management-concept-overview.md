---
title: Visão geral da API de gerenciamento de identidade e acesso do Azure AD
description: Use o Azure Active Directory (Azure AD) para gerenciar identidades e dispositivos e controlar o acesso em ambientes locais, híbridos e na nuvem.
author: jackson-woods
ms.localizationpriority: high
ms.prod: identity-and-access
ms.custom: scenarios:getting-started
ms.openlocfilehash: 85f1837c7e2c4b8a7d50000b14978645a9e247cd
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443792"
---
# <a name="azure-ad-identity-and-access-management-api-overview"></a>Visão geral da API de gerenciamento de identidade e acesso do Azure AD

O Active Directory do Azure (Azure AD) ajuda a centralizar o gerenciamento de identidade e acesso para permitir acesso seguro e produtivo entre aplicativos, dispositivos, serviços e infraestrutura. As organizações podem usar o Azure AD para gerenciar identidades e controlar o acesso em ambientes locais, híbridos e em nuvem.

Você pode usar as APIs REST do Azure AD no Microsoft Graph para criar fluxos de trabalho exclusivos entre os [recursos](/graph/api/resources/azure-ad-overview) do Azure AD e serviços de terceiros.

## <a name="why-use-the-azure-ad-apis"></a>Por que usar as APIs do Azure AD?

Mais de 15 milhões de organizações usam o Azure AD ao se inscreverem em serviços em nuvem da Microsoft, como o Microsoft 365, Microsoft Azure e Enterprise Mobility Suite.

Os desenvolvedores corporativos usam o Microsoft Graph para integrar o gerenciamento de identidades do Azure AD e outros serviços para automatizar fluxos de trabalho administrativos, como a integração (e rescisão) de funcionários, a manutenção de perfis, a implantação de licenças e muito mais.

Para muitos desenvolvedores corporativos, o Microsoft Graph e o Azure AD ajudam a "elevar e deslocar" os aplicativos existentes para a nuvem, acelerando a transformação digital de uma organização. Você pode aproveitar os recursos do Azure AD para adicionar mecanismos de controle de acesso a aplicativos, incluindo a verificação de associação de grupo, a função de diretório ou a associação de unidades administrativas de um usuário.

Você pode usar o Microsoft Graph e o Azure AD como uma maneira rápida e fácil de alcançar mais de 15 milhões de organizações, incluindo 90% das empresas da Fortune 500 que já usam os serviços do Azure AD. Os aplicativos integrados apresentam experiências de logon sem interrupções e podem usar dados organizacionais existentes para criar experiências personalizadas.

Você pode usar as APIs do Azure AD no Microsoft Graph para consultar o perfil do usuário, encontrar outros usuários, gerenciar relações organizacionais, rastrear atribuições ou criar soluções originais que incorporem dados organizacionais existentes. Essas APIs fornecem uma base sólida para integrar aplicativos de negócios personalizados aos serviços digitais existentes de uma organização.

### <a name="manage-users-and-groups"></a>Gerenciar usuários e grupos

Você pode usar as APIs do Azure AD no Microsoft Graph para:

- Pesquisar e gerenciar informações de [perfil de usuário](/graph/api/resources/user), como nome, foto, endereço de email, cargo, localização do escritório e muito mais de usuários na sua organização.
- Criar [grupos](/graph/api/resources/groups-overview) para projetos e equipes na sua organização. Adicionar e remover membros do grupo para controlar o acesso aos recursos. (Os grupos dinâmicos podem alterar automaticamente a associação com base nos valores da propriedade do usuário).
- Verifique a [associação transitiva](/graph/api/user-checkmembergroups) em uma lista de grupos ou obtenha todos os recursos de um tipo especificado (como usuário ou grupo) de uma lista de [ IDs de recursos genéricos ](/graph/api/directoryobject-getbyids) para controlar o acesso.

### <a name="manage-directory-roles"></a>Gerenciar funções de diretório

Você pode atribuir usuários a [funções de diretório](/graph/api/resources/directoryrole) administrativas predefinidas do Azure AD, que concede permissão para executar tarefas específicas.

### <a name="manage-devices"></a>Gerenciar dispositivos

[Gerenciar os dispositivos](/azure/active-directory/device-management-introduction) registrados na organização. Os dispositivos são registrados aos usuários e incluem itens como laptops, desktops, tablets e telefones celulares. Os dispositivos são geralmente criados na nuvem usando o Serviço de Registro de Dispositivos ou pela Microsoft Intune. Eles são utilizados por políticas de acesso condicional para autenticação multifator.

### <a name="partner-tenant-management"></a>Gerenciamento de locatário do parceiro

Os parceiros da Microsoft que revendem e gerenciam o Microsoft Online Services (como o Microsoft 365, o Microsoft Azure e o CRM Online) podem exibir os [locatários da organização](/graph/api/resources/contract) que gerenciam atualmente.

Você também pode [gerenciar domínios](/graph/api/resources/domain) associados a um locatário. As operações de domínio permitem que os parceiros da Microsoft automatizem o registro de domínio para serviços, como o Microsoft 365.

### <a name="tenant-management"></a>Gerenciamento de locatários

As APIs do Azure AD para o gerenciamento de locatários permitem:

- Obter informações sobre uma [organização](/graph/api/resources/organization), como seu endereço comercial, contatos de notificação e técnicos, assinaturas de serviço ativas e os domínios associados a ela.
- Obter informações sobre [SKUs do serviço](/graph/api/resources/subscribedsku) nos quais a empresa está inscrita.
- [Convidar usuários externos](/graph/api/resources/invitation) (convidados) para uma organização.

### <a name="monitor-identity-risks"></a>Monitorar riscos de identidade

A maioria das violações de segurança resulta de invasores que roubam a identidade do usuário. Os invasores tem sido muito eficientes em aproveitar de violações de terceiros, ataques de pulverização de senhas e ataques de phishing sofisticados. Isso significa que você precisa proteger todas as suas contas de usuário desses ataques e proativamente evitar identidades comprometidas de serem violadas.

O Azure AD usa algoritmos de aprendizado de máquina adaptativos e heurística para detectar anomalias que indicam potencialmente contas comprometidas. Com esses dados, o Azure Active Directory Identity Protection protege os usuários com políticas de acesso condicional baseadas em risco e gera relatórios e alertas com base em suas detecções.

Hoje, o Microsoft Graph oferece acesso fácil aos clientes do Azure AD Premium P2 para [consultar eventos de risco detectados pelo Identity Protection](/graph/api/resources/identityprotectionroot), incluindo o tipo do evento de risco, a gravidade, a data, a hora, o local, o usuário afetado e mais. Os clientes podem então usar esses eventos em sistemas SIEM e aplicativos de segurança.

### <a name="review-access-to-organizational-resources"></a>Analisar acesso aos recursos organizacionais

Analisar acesso a grupos, aplicações, e até mesmo papéis privilegiados em sua organização. [As análises de acesso](/graph/api/resources/accessreviews-root) são apresentadas no Azure AD Premium P2.

### <a name="activate-users-into-privileged-roles"></a>Ativar usuários em funções privilegiadas

Usar o [Gerenciamento de Identidade Privilegiado (PIM) API](/graph/api/resources/rolemanagement) para ativar o privilégio de administrador sob demanda. Forçar a justificação obrigatória da ativação de papéis, e autenticação multifatorial para os atores em papéis privilegiados.

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [API de gerenciamento de acesso e identidade do Azure AD no Microsoft Graph v1.0](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0&preserve-view=true)
- [API de gerenciamento de acesso e identidade do Azure AD no Microsoft Graph beta](/graph/api/resources/azure-ad-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>Próximas etapas

- Saiba como [Usar as APIs REST do Azure AD](/graph/api/resources/azure-ad-overview).
- Use o Azure AD para se [autenticar](./auth/index.yml) no Microsoft Graph.
- Integre o [logon do Azure AD](https://azure.microsoft.com/develop/identity/signin/) ao seu aplicativo ou website.
- Confira o [Changelog](changelog.md) para obter informações sobre novidades nas APIs do Azure AD.
- Explorar [exemplos](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples) para mais ideias sobre como usar o Microsoft Graph.
