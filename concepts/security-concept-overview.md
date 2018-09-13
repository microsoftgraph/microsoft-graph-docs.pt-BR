# <a name="microsoft-graph-security-api-overview"></a>Visão geral da API de segurança do Microsoft Graph

Você pode usar a API de segurança do Microsoft Graph para conectar produtos de segurança, serviços e parceiros da Microsoft para simplificar as operações de segurança e melhorar os recursos de proteção, detecção e resposta a ameaças. A API de segurança do Microsoft Graph é um serviço intermediário (ou broker) que fornece uma única interface programática para se conectar a vários [provedores de segurança do Microsoft Graph](../api-reference/v1.0/resources/securityvendorinformation.md) (também chamados de provedores de segurança provedores ou provedores). As solicitações para a API de segurança do Microsoft Graph estão alinhadas com todos os provedores de segurança aplicáveis. Os resultados são agregados e retornados para o aplicativo solicitante em um esquema comum, conforme mostrado no diagrama a seguir. Para obter detalhes, confira [Fluxo de dados de segurança do Microsoft Graph](security-dataflow.md).

![security_overview_diagram_1.PNG](./images/security_overview_diagram_1.png)

Para obter informações sobre autorização, confira [Autorização e a API de segurança](security-authorization.md). Para saber mais sobre permissões, incluindo permissões delegadas e de aplicativos, confira o artigo sobre [Permissões](permissions_reference.md#security-permissions).

## <a name="why-use-the-microsoft-graph-security-api"></a>Por que usar a API de segurança do Microsoft Graph?

A [API de segurança do Microsoft Graph](../api-reference/v1.0/resources/security-api-overview.md) facilita a conexão com diferentes produtos e serviços da Microsoft e de seus parceiros de segurança. Ele permite que você concretize e enriqueça o valor dessas soluções mais prontamente.

### <a name="unify-and-standardize-alert-tracking"></a>Unificação e padronização do acompanhamento de alertas

Escreva um único código para integrar os alertas de qualquer solução de segurança integrada do Microsoft Graph e mantenha alertas de status e atribuições sincronizados em todas as soluções. Também é possível transmitir alertas para soluções de gerenciamento de informações e eventos de segurança (SIEM) como Splunk e IBM QRadar por meio do [Azure Monitor](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). Para obter detalhes sobre a integração de SIEM com as entidades da API de segurança, consulte [Integração com uma SIEM](security_siemintegration.md).

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>Correlação de alertas de segurança para melhorar a proteção e a resposta a ameaças

Correlacione alertas em soluções de segurança mais facilmente com um esquema de alerta comum. Isso não só permite que você receba informações de alerta acionáveis como também permite que os analistas de segurança enriqueçam os alertas com informações e ativos de usuário, possibilitando uma resposta mais rápida às ameaças e proteção dos ativos.  

### <a name="update-alert-tags-status-and-assignments"></a>Atualização de etiquetas de alerta, status e tarefas

Adicione contexto ou inteligência contra ameaças aos alertas para instruir a resposta e a correção. Faça com que comentários e feedback sobre alertas tenham visibilidade em todos os fluxos de trabalho. Mantenha os status de alerta e atribuições em sincronia para que todas as soluções integradas reflitam o estado atual. Use assinaturas de webhooks para receber notificações de alteração.  

### <a name="unlock-security-context-to-drive-investigation"></a>Desvende o contexto de segurança para orientar a investigação

Aprofunde seus conhecimentos sobre inventários relevantes relacionados à segurança relevantes (como usuários, hosts e aplicativos) e adicione contexto organizacional de outros provedores do Microsoft Graph (Azure AD, Microsoft Intune, Office 365) para reunir os contextos comercial e de segurança e melhorar respostas a ameaças.

### <a name="proactively-manage-security-risks-preview"></a>Gerenciamento proativo de riscos de segurança (versão prévia)

Use o Microsoft Secure Score (versão prévia) para dar visibilidade às necessidades de segurança da sua organização e obter sugestões sobre como aperfeiçoá-la, e projete uma pontuação maior depois que essas sugestões forem incorporadas. Meça facilmente seu progresso ao longo do tempo e obtenha insights sobre as alterações específicas que geraram melhorias na sua pontuação.

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>Benefícios de usar a API de segurança do Microsoft Graph

A tabela a seguir lista os benefícios que diferentes soluções de segurança podem alcançar por meio da integração com a API de segurança do Microsoft Graph.  

|**Área**     | **Benefícios**|
|:---------------|:---------|
|**Provedores de serviços de segurança gerenciados (MSSPs)**|<ul><li>Integração simplificada com serviços e ferramentas de operações de segurança.</li> <li>Redução de tempo e esforços para implantação e manutenção.</li> <li>Capacidade de fornecer mais valor para clientes MSSP.</li></ul>|
|**SIEM e soluções de gerenciamento de risco de TI**|<ul><li>Integração perfeita com soluções de segurança da Microsoft e parceiros do ecossistema.</li> <li>Alertas com ricos metadados.</li> <li>Melhor correlação de alertas.</li></ul>|
|**Aplicativos** <br> (Inteligência contra ameaças, dispositivos móveis, nuvem, IOT, detecção de fraudes, identidade e acesso, riscos e conformidade, firewall e assim por diante)|<ul><li>Gerenciamento unificado contra ameaças, prevenção e gerenciamento de riscos entre várias soluções de segurança.</li> <li>Alertas, inventário, configuração e ações expostas por meio do Microsoft Graph.</li> <li>Integração instantânea com soluções habilitadas com o Microsoft Graph.</li></ul>|

## <a name="next-steps"></a>Próximas etapas

- [Utilização da API de segurança do Microsoft Graph](../api-reference/v1.0/resources/security-api-overview.md)
- Está interessado em se tornar um provedor de segurança? Acesse [graphsecfeedback](mailto:graphsecfeedback@microsoft.com).
