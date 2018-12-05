---
title: Visão geral da API de Segurança do Microsoft Graph
description: Você pode usar a API de Segurança do Microsoft Graph para se conectar aos produtos, serviços e parceiros de segurança da Microsoft para simplificar operações de segurança e melhorar a proteção contra ameaças, a detecção de ameaças e a capacidade de resposta. A API de Segurança do Microsoft Graph é um serviço (ou agente) intermediário que proporciona uma interface de programação única para conectar diversos provedores de Segurança do Microsoft Graph (também chamados provedores de segurança ou provedores). As solicitações para a API de Segurança do Microsoft Graph são federadas para todos os provedores de segurança aplicáveis. Os resultados são agregados e retornam ao aplicativo solicitantes em um esquema comum, como mostrado no diagrama a seguir. Para saber detalhes, confira o fluxo de dados da API de Segurança do Microsoft Graph.
ms.openlocfilehash: b5e1fb3d60cfc55cb940a217aaba872175887297
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091561"
---
# <a name="microsoft-graph-security-api-overview"></a>Visão geral da API de Segurança do Microsoft Graph

Você pode usar a API de Segurança do Microsoft Graph para se conectar aos produtos, serviços e parceiros de segurança da Microsoft para simplificar operações de segurança e melhorar a proteção contra ameaças, a detecção de ameaças e a capacidade de resposta. A API de Segurança do Microsoft Graph é um serviço (ou agente) intermediário que proporciona uma interface de programação única para conectar diversos [provedores de Segurança do Microsoft Graph](/graph/api/resources/securityvendorinformation?view=graph-rest-1.0) (também chamados provedores de segurança ou provedores). As solicitações para a API de Segurança do Microsoft Graph são federadas para todos os provedores de segurança aplicáveis. Os resultados são agregados e retornam ao aplicativo solicitantes em um esquema comum, como mostrado no diagrama a seguir. Para saber detalhes, confira o[ fluxo de dados da API de Segurança do Microsoft Graph](security-dataflow.md).

![security_overview_diagram_1.png](./images/security-overview-diagram-1.png)

Para informações sobre autorização, confira [Autorização e a API de Segurança do Microsoft Graph](security-authorization.md). Para saber mais sobre permissões, incluindo permissões delegadas e de aplicativos, confira [Permissões](permissions-reference.md#security-permissions).

## <a name="why-use-the-microsoft-graph-security-api"></a>Por que usar a API de Segurança do Microsoft Graph?

A [API de Segurança do Microsoft Graph](/graph/api/resources/security-api-overview?view=graph-rest-1.0) facilita a conexão com diferentes produtos e serviços de segurança da Microsoft e de seus parceiros. Ela permite que você entenda e enriqueça mais rapidamente o valor dessas soluções.

### <a name="unify-and-standardize-alert-tracking"></a>Unificar e padronizar o monitoramento de alertas

Escreva o código uma vez para integrar os alertas de qualquer solução de segurança integrada do Microsoft Graph e mantenha os status de alerta e as atribuições sincronizados em todas as soluções. Também é possível transmitir alertas para soluções de informações de segurança e gerenciamento de eventos (SIEM), como Splunk e IBM QRadar, através do [Azure Monitor](https://docs.microsoft.com/pt-BR/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). Para saber mais sobre a integração de SIEM com entidades da API de segurança, consulte [Integração com SIEM](security-siemintegration.md).

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>Correlacionar alertas de segurança para melhorar a resposta e a proteção contra ameaças

Correlacione alertas em soluções de segurança mais facilmente com um esquema de alerta unificado. Além de permitir que você receba informações de alerta acionáveis, permite também que analistas de segurança dinamizem e enriqueçam alertas com informações de ativos e usuários, possibilitando uma resposta mais rápida a ameaças e a proteção dos ativos.  

### <a name="update-alert-tags-status-and-assignments"></a>Atualizar marcas, status e atribuições de alerta

Marque os alertas com contexto adicional ou inteligência contra ameaças para informar a resposta e a correção. Certifique-se de que os comentários e as opiniões nos alertas sejam capturados e estejam visíveis em todos os fluxos de trabalho. Mantenha as atribuições e o status de alerta sincronizados para que todas as soluções integradas reflitam o estado atual. Use assinaturas webhook para receber notificação das alterações.  

### <a name="unlock-security-context-to-drive-investigation"></a>Desbloquear o contexto de segurança para orientar investigação

Aprofunde seus conhecimentos sobre inventários relevantes relacionados à segurança relevantes (como usuários, hosts e aplicativos) e adicione contexto organizacional de outros provedores do Microsoft Graph (Azure AD, Microsoft Intune, Office 365) para reunir os contextos comercial e de segurança e melhorar respostas a ameaças.

### <a name="proactively-manage-security-risks-preview"></a>Gerenciar proativamente riscos de segurança (visualização)

Use o Microsoft Secure Score (visualização) para proporcionar visibilidade às necessidades de segurança de sua organização e obter sugestões sobre como melhorá-las, além de projetar uma pontuação melhorada depois dessas sugestões serem implementadas. Meça facilmente seu progresso ao longo do tempo e obtenha ideias sobre alterações específicas que conduziram à melhoria de sua pontuação.

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>Benefícios do uso da API de Segurança do Microsoft Graph

A tabela a seguir lista os benefícios que as diferentes soluções de segurança podem acessar ao se integrar com a API de Segurança do Microsoft Graph.  

|**Área**     | **Benefícios**|
|:---------------|:---------|
|**Gerenciamento de Provedores de Serviços de Segurança (MSSPs)**|<ul><li>Integração simplificada com ferramentas e serviços de operações de segurança.</li> <li>Redução no tempo e no esforço de implantação e manutenção.</li> <li>Capacidade de oferecer mais vantagens para os clientes MSSP.</li></ul>|
|**Soluções de gerenciamento de risco de TI e SIEM**|<ul><li>Integração perfeita com soluções de segurança da Microsoft e ecossistemas parceiros.</li> <li>Metadados de alerta avançados.</li> <li>Melhor correlação de alerta.</li></ul>|
|**Aplicativos** <br>(Inteligência contra Ameaças, Celular, Nuvem, IOT, Detecção de Fraudes, Identidade e Acesso, Risco e Conformidade, Firewall e muito mais)|<ul><li>Gerenciamento unificado de ameaças, prevenção e gerenciamento de riscos em diversas soluções de segurança.</li> <li>Alertas, estoque, configuração e ações expostas através do Microsoft Graph.</li> <li>Integração instantânea com soluções habilitadas pelo Microsoft Graph.</li></ul>|

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [API de Segurança no Microsoft Graph v1.0](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- [API de Segurança na versão beta do Microsoft Graph](/graph/api/resources/security-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Segurança do Microsoft Graph](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- Interessado em se tornar um provedor de segurança? Contate [graphsecfeedback](mailto:graphsecfeedback@microsoft.com).
