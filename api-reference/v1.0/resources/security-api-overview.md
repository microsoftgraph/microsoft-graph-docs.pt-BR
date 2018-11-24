# <a name="use-the-microsoft-graph-security-api"></a>Usar a API de segurança do Microsoft Graph

A API de segurança do Microsoft Graph fornece uma interface unificada e o esquema de integrar com as soluções de segurança da Microsoft e ecossistema de parceiros. Isso permite que os clientes simplificar as operações de segurança e proporcionando melhor defesa contra ameaças de aumento. A API de segurança do Microsoft Graph pode ser usada como um serviço de agregação de lista segura de segurança federada enviem consultas ao todos os provedores de segurança onboarded para obter respostas agregadas. Use a API de segurança do Microsoft Graph para criar aplicativos que:

- Consolide e correlacionar os alertas de segurança de várias fontes
- Desbloquear dados contextuais para informar investigações
- Automatize as operações de segurança para maior eficiência
- Fornecer dados de segurança para habilitar o gerenciamento de riscos proativo de visibilidade

A API de segurança do Microsoft Graph inclui as seguintes entidades principais.

## <a name="alerts"></a>Alertas

Alertas são possíveis problemas de segurança dentro do locatário do cliente que as soluções de segurança da Microsoft ou parceiro identificaram e são marcadas para ação ou notificação. Com a entidade de [alertas](alert.md) de segurança do Microsoft Graph, você pode unificar e agilizar os problemas de segurança em todas as soluções integradas. Isso também permite que aplicativos correlacionar contexto para melhorar a resposta e a proteção contra ameaças e alertas. Essas desbloquear eficiência operacional de segurança, reduzindo o tempo de investigação e tempo resolução de incidentes. Com o recurso de atualização de alerta, você pode sincronizar o status dos alertas específicos entre produtos de segurança diferentes e serviços que são integrados com a API de segurança do Microsoft Graph Atualizando sua entidade [alertas](alert.md) .

Soluções do Microsoft Graph segurança integrada receberá alertas dos seguintes provedores de segurança:

- Central de segurança do Windows Azure
- Proteção de identidade do Azure Active Directory
- Proteção das informações do Azure
- Segurança de aplicativo de nuvem da Microsoft
- Proteção de ameaça avançada do Windows Defender
- Microsoft Intune (privada preview)
- Office 365 (em breve)
- Azure avançada proteção contra ameaças (em breve)
- Soluções de parceiros, como Palo Alto redes App Framework

> **Observação:** Novos provedores são continuamente inclusão para o ecossistema de segurança do Microsoft Graph.

## <a name="common-use-cases"></a>Casos comuns de uso

A seguir estão algumas das solicitações mais populares para trabalhar com a API de segurança do Microsoft Graph:

| **Casos de uso**   | **Recursos REST** | **Experimente no Explorer do gráfico** |
|:---------------|:--------|:----------|
| Listar alertas | [Listar alertas](../api/alert_list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| Atualizar alertas | [Atualizar alertas](../api/alert_update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

Você pode usar o Microsoft Graph [webhooks](../../../concepts/webhooks.md) se inscrever e receber notificações sobre atualizações para entidades de segurança do Microsoft Graph.

## <a name="resources"></a>Recursos

Código e contribuem para esses exemplos de API do Microsoft Graph segurança:

- [Amostra do ASP.NET (c#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Amostra de Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Amostra de Node. js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Participe da comunidade:

- [Ingressar na comunidade do tech](https://aka.ms/graphsecuritycommunity)
- [Discuta no StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>Próximas etapas

A API de segurança do Microsoft Graph pode aberto novas maneiras para que você entre em contato com as soluções de segurança diferente da Microsoft e parceiros. Siga estas etapas para começar:

- Detalhar [alertas](alert.md).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer). Em **Exemplos de consultas**, escolha **Mostrar mais exemplos** e defina a categoria de segurança para **ativado**.
- Tente [inscritos para e recebe notificações](../../../concepts/webhooks.md) sobre alterações de entidade.

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).
