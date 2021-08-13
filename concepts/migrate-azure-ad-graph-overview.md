---
title: Migrar aplicativos do Azure AD Graph microsoft Graph
description: Descreve como migrar aplicativos de API Azure Active Directory (Azure AD) para a API Graph Microsoft.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 2eba88d5995d44098473ad138d65df8650cbddb350ad401f731238b8c381be2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163513"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>Migrar aplicativos do Azure AD Graph microsoft Graph

O Microsoft Graph está substituindo totalmente Azure Active Directory (Azure AD) Graph. Para a maioria dos aplicativos de produção, o Microsoft Graph já pode suportar totalmente os cenários do Azure AD. Você deve começar a mover seus aplicativos do Azure AD Graph microsoft Graph agora.

Além disso, o Microsoft Graph oferece suporte a muitos novos conjuntos de dados e recursos do Azure AD que não estão disponíveis no Azure AD Graph. Alterne para a Microsoft Graph aproveitar essas novas APIs, tudo por meio de um único ponto de extremidade, incluindo:

- [Microsoft 365 gerenciamento de grupo](/graph/office365-groups-concept-overview).
- [Convites de usuário externos](/graph/api/resources/invitation?view=graph-rest-1.0).
- A capacidade de [restaurar usuários e Microsoft 365 grupos depois](/graph/api/resources/directory?view=graph-rest-1.0) que eles foram excluídos.
- [Notificações de webhook em usuários e grupos](/graph/webhooks?toc=./ref/toc.json&view=graph-rest-1.0).
- Recursos de governança de identidade, como:
  - [PiM (gerenciamento de](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) identidade privilegiada) para elevar os usuários a funções privilegiadas somente quando necessário e por um período limitado.
  - [Acesse análises de](/graph/api/resources/accessreviews-root?view=graph-rest-beta) acesso para análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário.
  - [Termos de uso para permitir que](/graph/api/resources/accessreviews-root?view=graph-rest-beta) as organizações apresentem informações para requisitos legais ou de conformidade, como avisos de isenção de responsabilidade.
- Recursos de segurança como:
  - [Eventos de risco de identidade](/graph/api/resources/identityriskevent?view=graph-rest-beta).
  - [Usuários arriscados](/graph/api/resources/riskyuser?view=graph-rest-beta).
- [Bibliotecas de clientes e exemplos](/graph/) disponíveis em muitas outras plataformas e idiomas. Os SDKs do Microsoft Graph fornecem uma interface descobrivel para acessar facilmente seus dados enquanto manipulam de forma transparente a aquisição de tokens, a manipulação de novo devido a erros e a throttling, tratamento seguro de redirecionamento e serialização de modelo e dessarialização.

O Microsoft Graph oferece acesso a muito mais serviços do que apenas Azure Active Directory. É o gateway [da API para Microsoft 365 serviços também.](/graph/)

O restante dos artigos nesta seção ajudam você a mover seu aplicativo do Azure AD Graph para o Microsoft Graph. Você encontrará:

- Uma lista de verificação para ajudá-lo a planejar.
- Diretrizes que descrevem diferenças específicas entre as APIs.
- Links para recursos adicionais e exemplos para ilustrar diferenças específicas.
- Perguntas frequentes para resolver outras perguntas ou preocupações


## <a name="frequently-asked-questions-faq"></a>Perguntas frequentes (FAQ)

### <a name="is-azure-ad-graph-aad-graph-deprecated"></a>O Azure AD Graph (AAD Graph) preterido?  
Sim. A partir de 30 de junho de 2020, não adicionaremos mais novos recursos ao AAD Graph. Continuaremos adicionando correções críticas de segurança até 30 de junho de 2022. As APIs não funcionarão mais corretamente após 30 de junho de 2022.

### <a name="how-do-i-know-which-of-my-apps-are-using-aad-graph"></a>Como saber quais dos meus aplicativos estão usando o AAD Graph?  
Os aplicativos devem ser registrados para usar o AAD Graph.  Você pode ver a página Registro de Aplicativo no Portal de Locatários do Azure para ver se um determinado aplicativo está registrado para usar o AAD Graph.

### <a name="how-do-i-know-which-apis-my-applications-are-calling"></a>Como saber quais APIs meus aplicativos estão chamando?
Se você tiver o código-fonte do aplicativo, poderá fazer referência às guias de migração nesta seção para ajudar a determinar quais APIs o aplicativo usa e como migrá-lo para o Microsoft Graph. Se você não tiver acesso ao código-fonte [](developer-support-help-options.md#open-a-support-request) do aplicativo, poderá abrir uma solicitação de suporte para obter uma lista das APIs que cada aplicativo está chamando.

### <a name="will-my-existing-aad-graph-apps-continue-to-work"></a>Meus aplicativos existentes do AAD Graph continuarão a funcionar? 
Seus aplicativos existentes continuarão a funcionar sem modificação até 30 de junho de 2022. A FUNÇÃO E Graph API do AAD após esse tempo não é garantido.

### <a name="why-should-i-invest-in-moving-to-microsoft-graph"></a>Por que devo investir na mudança para a Microsoft Graph?  
O Microsoft Graph é o gateway para dados e inteligência no Microsoft 365. Ele fornece um modelo de programação unificado que você pode usar para acessar a quantidade enorme de conjuntos de dados e recursos no Microsoft 365, Azure, Windows 10 e Enterprise Mobility + Security. Você pode usar a riqueza de dados no Microsoft Graph para criar e gerenciar aplicativos para organizações de qualquer escala.

### <a name="will-you-release-a-tool-that-helps-me-move-my-apps-from-aad-graph-to-microsoft-graph"></a>Você liberará uma ferramenta que me ajude a mover meus aplicativos do AAD Graph para o Microsoft Graph?  
Embora não temos ferramentas para anunciar no momento, estamos sempre trabalhando para melhorar a experiência da plataforma de nossos desenvolvedores. Isso inclui o fornecimento de ferramentas e dados para facilitar a manutenção dos aplicativos atuais com alterações na API.

### <a name="how-do-i-get-help-migrating-my-application"></a>Como posso obter ajuda para migrar meu aplicativo?  
Consulte a seção Próximas Etapas deste artigo. Se depois de ler você tiver perguntas adicionais, poderá postar em Stack Overflow com a marca ou abrir um problema no repositório de GitHub `[aadgraph-deprecation]` [da API.](https://github.com/microsoftgraph)


## <a name="next-steps"></a>Próximos passos

- Ande pela lista de verificação [de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md) para ajudá-lo a planejar a movimentação.
- Explore os Graph e práticas da [Microsoft.](/graph/overview)
- Use [Graph Explorer para](https://aka.ms/ge) experimentar com o Microsoft Graph.
- Para saber mais sobre atualizações de progresso e cronogramas, consulte [Microsoft Graph ou o Azure AD Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/).

