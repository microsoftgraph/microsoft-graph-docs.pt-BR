---
title: Migrar aplicativos do Azure AD Graph microsoft Graph
description: Descreve como migrar aplicativos de API Azure Active Directory (Azure AD) para a API Graph Microsoft.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 100fa23b9fdd7b82e201ed2fc6139f62ca93f74c
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651278"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a>Migrar aplicativos do Azure AD Graph microsoft Graph

> [!WARNING]
> **Azure Active Directory (Azure AD) Graph está preterido**. Para evitar a perda de funcionalidade, migre seus aplicativos para o Microsoft Graph antes de 30 de junho de 2022, quando os pontos de extremidade da API do Azure AD Graph deixarão de responder às solicitações.
>
> A Microsoft continuará com o suporte técnico e aplicará correções de segurança para o Azure AD Graph até 30 de junho de 2022, quando todas as funcionalidades e suporte terminarão. Se você não migrar seus aplicativos para a Microsoft Graph antes de 30 de junho de 2022, você colocará sua funcionalidade e estabilidade em risco.

[O Azure AD Graph está preterido.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/update-your-applications-to-use-microsoft-authentication-library/ba-p/1257363) Atualize seus aplicativos do Azure AD Graph usar o Microsoft Graph agora.

## <a name="why-use-microsoft-graph"></a>Por que usar o Microsoft Graph?

O Azure AD Graph oferece acesso apenas aos serviços do Azure AD. A Microsoft Graph oferece um único ponto de extremidade unificado para acessar os serviços do Azure AD e outros serviços Microsoft 365, como Microsoft Teams, Microsoft Exchange e Microsoft Intune. Para a maioria dos aplicativos de produção, o Microsoft Graph oferece suporte total aos cenários do Azure AD.

O Microsoft Graph também é mais seguro e resiliente do que o Azure AD Graph.

Além disso, o Microsoft Graph oferece suporte a muitos novos conjuntos de dados e recursos do Azure AD que não estão disponíveis no Azure AD Graph, incluindo no Windows 10 e Enterprise Mobility + Security (EMS). Alterne para a Microsoft Graph aproveitar essas novas APIs, tudo por meio de um único ponto de extremidade, incluindo:

- [Microsoft 365 gerenciamento de grupo](/graph/office365-groups-concept-overview).
- [Convites de usuário externos](/graph/api/resources/invitation).
- A capacidade de [restaurar usuários, Microsoft 365 grupos, aplicativos](/graph/api/resources/directory) e entidades de serviço após a exclusão.
- [Notificações de webhook em usuários e grupos](/graph/webhooks).
- Recursos avançados de gerenciamento de licenças, incluindo [licenciamento baseado em grupo.](/graph/api/group-assignlicense)
- Recursos de governança de identidade, como:
  - [PiM (gerenciamento de](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta&preserve-view=true) identidade privilegiada) para elevar os usuários a funções privilegiadas somente quando necessário e por um período limitado.
  - [Acesse análises de](/graph/api/resources/accessreviewsv2-overview) acesso para análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário.
  - [Termos de uso para permitir que](/graph/api/resources/agreement) as organizações apresentem informações para requisitos legais ou de conformidade, como avisos de isenção de responsabilidade.
- Recursos de segurança como:
  - [Eventos de risco de identidade](/graph/api/resources/riskdetection).
  - [Usuários arriscados](/graph/api/resources/riskyuser).
- [Bibliotecas de clientes e exemplos](/graph/) disponíveis em muitas outras plataformas e idiomas. Os SDKs do Microsoft Graph fornecem uma interface descobrivel para acessar facilmente seus dados enquanto manipulam de forma transparente a aquisição de tokens, a manipulação de novo devido a erros e a throttling, tratamento seguro de redirecionamento e serialização de modelo e dessarialização.
- Mais [recursos de consulta OData suportados](/graph/query-parameters) por recursos como usuários, grupos, aplicativos e entidades de serviço.

O restante dos artigos nesta seção ajudam você a migrar seu aplicativo do Azure AD Graph para o Microsoft Graph. Você encontrará:

- Uma lista de verificação para ajudá-lo a planejar a migração.
- Diretrizes que descrevem diferenças específicas entre as APIs.
- Links para mais recursos e exemplos para ilustrar diferenças específicas.
- Uma perguntas frequentes para resolver outras perguntas ou preocupações.

## <a name="next-steps"></a>Próximas etapas

- Ande pela lista de verificação [de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md) para ajudá-lo a planejar a migração.
- Explore os Graph e práticas da [Microsoft.](/graph/overview)
- Use [Graph Explorer para](https://aka.ms/ge) experimentar com o Microsoft Graph.
- Para saber mais sobre atualizações de progresso e cronogramas, consulte [Microsoft Graph ou o Azure AD Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/).
- Obter [respostas para perguntas](/graph/migrate-azure-ad-graph-faq) que você pode ter sobre a migração.