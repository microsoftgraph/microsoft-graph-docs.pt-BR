# <a name="overview-of-security-in-microsoft-graph-preview"></a>Visão geral de segurança no Microsoft Graph (prévia) 

Você pode usar o Microsoft Graph para se conectar com o Intelligent Security Graph para tirar proveito dos recursos da Microsoft e dos parceiros de segurança, e criar melhores soluções de resposta a ameaças. O Microsoft Graph também fornece acesso aos riscos de usuário e conta detectados pelo serviço Identity Protection no Azure Active Directory (Azure AD), permitindo a integração de dados de risco de conta em seus aplicativos de segurança.

## <a name="why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph"></a>Por que usar a API de segurança e se conectar com o Gráfico de Segurança Inteligente da Microsoft?

O Intelligent Security Graph é uma plataforma unificada de combate a ciberataques. Ela tem proteção a ameaças em tempo real para produtos e serviços Microsoft e é compatível com um ecossistema de soluções integradas.

A [API de segurança do Microsoft Graph](https://aka.ms/graphsecuritydocs) facilita a conexão com essas soluções no Intelligent Security Graph. Permite que você mais rapidamente perceba e valorize essas soluções.

### <a name="unify-and-standardize-alert-management"></a>Unificar e padronizar o gerenciamento de alertas

Correlacione alertas em soluções de segurança mais facilmente com um esquema de alerta comum. Escreva código uma vez para integrar os alertas de qualquer solução de segurança integrada do Microsoft Graph e mantenha em sincronizados os status de alerta e as atribuições em todas as soluções. Também é possível transmitir alertas a soluções de gerenciamento de informações e eventos de segurança (SIEM) como Splunk e IBM QRadar por meio do [Azure Monitor](https://docs.microsoft.com/pt-BR/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub).

### <a name="federated-security-aggregation-service"></a>Serviço de agregação de segurança federado

Use a API de segurança como um serviço de agregação de segurança federado para enviar consultas a todos os provedores de segurança participantes e obter respostas agregadas.

### <a name="unlock-security-context-to-drive-investigation"></a>Desbloquear o contexto de segurança para orientar investigação

Aprofunde seus conhecimentos sobre inventários relevantes relacionados à segurança relevantes (como usuários, hosts e aplicativos) e adicione contexto organizacional de outros provedores do Microsoft Graph (Azure AD, Microsoft Intune, Office 365) para reunir os contextos comercial e de segurança e melhorar respostas a ameaças.

## <a name="why-use-azure-ad-to-protect-identities-in-your-organization"></a>Por que usar o Azure AD para proteger identidades em sua organização?

A maioria das violações de segurança resulta de invasores que roubam a identidade do usuário. Os invasores tem sido muito eficientes em aproveitar de violações de terceiros, ataques de pulverização de senhas e ataques de phishing sofisticados. Isso significa que você precisa proteger todas as suas contas de usuário desses ataques e proativamente evitar identidades comprometidas de serem violadas.

O Azure AD usa algoritmos de aprendizado de máquina adaptativos e heurística para detectar anomalias que indicam potencialmente contas comprometidas. Com esses dados, o Identity Protection protege os usuários com políticas de acesso condicional baseadas em risco e gera relatórios e alertas com base em suas detecções.

Hoje, o Microsoft Graph fornece acesso fácil a clientes P1 e P2 do Azure AD Premium a detecções de risco feitas pelo Identity Protection e usa esses eventos em sistemas SIEM e aplicativos de segurança.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de segurança](../api-reference/beta/resources/security-api-overview.md)
- [Usar a API do Azure AD Identity Protection](../api-reference/beta/resources/identityprotection_root.md)

