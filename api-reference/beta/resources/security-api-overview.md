---
title: Usar a API de Segurança do Microsoft Graph
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: dff91665fc288bf1714d1975f3ec2e109f576530
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184529"
---
# <a name="use-the-microsoft-graph-security-api"></a>Usar a API de Segurança do Microsoft Graph

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

A API de segurança do Microsoft Graph fornece uma interface unificada e o esquema de integrar com as soluções de segurança da Microsoft e ecossistema de parceiros. Isso permite que os clientes simplificar as operações de segurança e proporcionando melhor defesa contra ameaças de aumento. A API de segurança do Microsoft Graph pode ser usada como um serviço de agregação de lista segura de segurança federada enviem consultas ao todos os provedores de segurança onboarded para obter respostas agregadas. Use a API de segurança do Microsoft Graph para criar aplicativos que:

- Consolide e correlacionar os alertas de segurança de várias fontes
- Desbloquear dados contextuais para informar investigações
- Automatize as operações de segurança para maior eficiência
- Fornecer dados de segurança para habilitar o gerenciamento de riscos proativo de visibilidade

A API de segurança do Microsoft Graph inclui as seguintes entidades principais.

## <a name="alerts"></a>Alertas

Alertas são possíveis problemas de segurança dentro do locatário do cliente que as soluções de segurança da Microsoft ou parceiro identificaram e são marcadas para ação ou notificação. Com a entidade de [alertas](alert.md) de segurança do Microsoft Graph, você pode unificar e agilizar os problemas de segurança em todas as soluções integradas. Isso também permite que aplicativos correlacionar contexto para melhorar a resposta e a proteção contra ameaças e alertas. Essas desbloquear eficiência operacional de segurança, reduzindo o tempo de investigação e tempo resolução de incidentes. Com o recurso de atualização de alerta, você pode sincronizar o status dos alertas específicos entre produtos de segurança diferentes e serviços que são integrados com a API de segurança do Microsoft Graph Atualizando sua entidade [alertas](alert.md) .

Soluções do Microsoft Graph segurança integrada receberá alertas dos seguintes provedores de segurança:

- [Central de segurança do Windows Azure](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Proteção de identidade do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Segurança de aplicativo de nuvem da Microsoft](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [Proteção de ameaça avançada do Windows Defender](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- [Proteção das informações do Azure](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(preview)**
- Microsoft Intune **(privada preview)**
- O Office 365 **(em breve)**
- Azure de proteção de ameaça avançadas **(em breve)**
- Soluções de parceiros, como Palo Alto redes App Framework

> **Observação:** Novos provedores são continuamente inclusão para o ecossistema de segurança do Microsoft Graph.

## <a name="secure-score-preview"></a>Seguro pontuação (preview)

[Pontuação de seguro da Microsoft](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358) é uma solução de análise de segurança que dá a visibilidade seu portfólio de segurança e como aperfeiçoá-lo. Com uma única pontuação, você pode compreender melhor o que você fez para reduzir o risco no Microsoft solutions. Você também pode comparar sua pontuação com outras organizações e ver como sua pontuação tiver sido tendências ao longo do tempo. As entidades de segurança do Microsoft Graph [secureScore](securescores.md) e [secureScoreControlProfiles](securescorecontrolprofiles.md) ajudarão-lo a equilibrar as necessidades da sua organização de segurança e a produtividade, permitindo a combinação apropriada dos recursos de segurança. Você também pode projetar sua pontuação que seria depois que você adotar os recursos de segurança.

## <a name="common-use-cases"></a>Casos comuns de uso

A seguir estão algumas das solicitações mais populares para trabalhar com a API de segurança do Microsoft Graph.

| **Casos de uso**   | **Recursos REST** | **Experimente no Explorer do gráfico** |
|:---------------|:--------|:----------|
| Listar alertas | [Listar alertas](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| Atualizar alertas | [Atualizar alertas](../api/alert-update.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) |
|Lista as pontuações de seguro|[Lista secureScores](../api/securescores-list.md) (preview)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Lista de perfis de controle de pontuação de seguro|[Lista secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) (preview)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Atualização de perfis de controle de pontuação de seguro|[Atualizar secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md) (preview)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

Você pode usar o Microsoft Graph [webhooks](/graph/webhooks) se inscrever e receber notificações sobre atualizações para entidades de segurança do Microsoft Graph.

## <a name="next-steps"></a>Próximas etapas

A API de segurança do Microsoft Graph pode aberto novas maneiras para que você entre em contato com as soluções de segurança diferente da Microsoft e parceiros. Siga estas etapas para começar:

- Detalhar os [alertas](alert.md), [secureScore](securescores.md) (Preview) e [secureScoreControlProfiles](securescorecontrolprofiles.md) (Preview).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer). Em **Exemplos de consultas**, escolha **Mostrar mais exemplos** e defina a categoria de segurança para **ativado**.
- Tente [inscritos para e recebe notificações](/graph/webhooks) sobre alterações de entidade.

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

## <a name="see-also"></a>Confira também

Código e contribuem para esses exemplos de API do Microsoft Graph segurança:

- [Amostra do ASP.NET (c#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Amostra de Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Amostra de Node. js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Participe da comunidade:

- [Ingressar na comunidade do tech](https://aka.ms/graphsecuritycommunity)
- [Discuta no StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)
