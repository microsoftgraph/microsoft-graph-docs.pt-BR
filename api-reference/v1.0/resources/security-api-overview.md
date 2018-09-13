# <a name="use-the-microsoft-graph-security-api"></a>Use a API de segurança do Microsoft Graph

A API de segurança do Microsoft Graph fornece uma interface e um esquema unificados para integração com soluções de segurança da Microsoft e de parceiros do ecossistema. Isso capacita os clientes a agilizar as operações de segurança e a se defender melhor contra o aumento de ameaças cibernéticas. A API de segurança do Microsoft Graph pode ser usada como um serviço de agregação de segurança federada para enviar consultas a todos os provedores de segurança integrados para obter respostas agregadas. Use a API de segurança do Microsoft Graph para criar aplicativos que:

- Consolide e correlacione os alertas de segurança de várias fontes
- Desbloqueie dados contextuais para informar investigações
- Automatize as operações de segurança para maior eficiência
- Forneça visibilidade dos dados de segurança para permitir o gerenciamento proativo de riscos

A API de segurança do Microsoft Graph inclui as seguintes entidades principais.

## <a name="alerts"></a>Alertas

Alertas são possíveis problemas de segurança no locatário de um cliente que a Microsoft ou soluções de segurança de parceiros identificaram e estão sinalizadas para ação ou notificação. Com a entidade de segurança  [alertas](alert.md) do Microsoft Graph, você pode unificar e simplificar os problemas de segurança em todas as soluções integradas. Isso também permite que os aplicativos correlacionem alertas e contexto para melhorar a proteção e a resposta a ameaças. Isso libera eficiências operacionais de segurança, reduzindo o tempo de investigação e o tempo de resolução de incidentes. Com o recurso de atualização de alerta, você pode sincronizar o status de alertas específicos em diferentes produtos e serviços de segurança integrados com a API de segurança do Microsoft Graph, atualizando sua entidade [alertas](alert.md) .

As soluções integradas à segurança do Microsoft Graph receberão alertas dos seguintes provedores de segurança:

- Central de segurança do Windows Azure
- Proteção de identidade do Active Directory do Azure
- Proteção de Informações do Azure
- Segurança de aplicativo na nuvem da Microsoft
- Proteção Avançada Contra Ameaças do Windows Defender
- Microsoft Intune (versão prévia privada)
- Office 365 (em breve)
- Soluções de parceiros, como Palo Alto Networks App Framework

> **Observação:** Novos provedores estão continuamente participando do ecossistema do Microsoft Graph Security.

## <a name="common-use-cases"></a>Casos de uso comuns

A seguir estão algumas das solicitações mais populares para trabalhar com a API de segurança do Microsoft Graph:

| **Casos de uso**   | **Recursos REST** | **Experimentar no Graph Explorer** |
|:---------------|:--------|:----------|
| Listar alertas | [Listar alertas](../api/alert_list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| Atualizar alertas | [Atualizar alertas](../api/alert_update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

Você pode usar o [webhooks](../../../concepts/webhooks.md) do Microsoft Graph se inscrever e receber notificações sobre atualizações para entidades de segurança do Microsoft Graph.

## <a name="resources"></a>Recursos

Codifique e contribua para esses exemplos de API de segurança do Microsoft Graph:

- [Amostra de ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Amostra de Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Amostra de Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Participe da comunidade:

- [Participe da comunidade](https://aka.ms/graphsecuritycommunity)
- [Discuta no StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>Próximas etapas

A API de segurança do Microsoft Graph pode abrir novas formas para você se envolver com diferentes soluções de segurança da Microsoft e de parceiros. Siga estas etapas para começar:

- Detalhar [alertas](alert.md).
- Experimente a API no [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer). Em **Exemplos de consultas**, escolha **mostrar mais exemplos** e defina a categoria de segurança para **on**.
- Tente [inscrever-se e receber notificações](../../../concepts/webhooks.md) sobre mudanças na entidade.

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).
