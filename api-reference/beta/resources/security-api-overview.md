---
title: Usar a API de Segurança do Microsoft Graph
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.localizationpriority: high
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7c45ed1f157dbd634eb27fc633deb41ee996f2b6
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855886"
---
# <a name="use-the-microsoft-graph-security-api"></a>Usar a API de Segurança do Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A API de Segurança do Microsoft Graph fornece uma interface unificada e um esquema para integrar soluções de segurança da Microsoft e parceiros de ecossistema. Isso permite aos clientes agilizar as operações de segurança e a se proteger melhor contra as crescentes ameaças cibernéticas. A API de segurança do Microsoft Graph consulta todos os provedores de segurança integrados e agrega respostas. Use a API de Segurança do Microsoft Graph para compilar aplicativos que:

- Consolidem e correlacionem alertas de segurança de várias fontes
- Desbloqueiem dados contextuais para informar investigações
- Automatizem tarefas de segurança, processos de negócios, fluxos de trabalho e relatórios
- Enviem indicadores de ameaças para produtos da Microsoft para detecções personalizados
- Usem ações em resposta à novas ameaças
- Dão visibilidade aos dados de segurança para permitir o gerenciamento proativo dos riscos

A API de Segurança do Microsoft Graph inclui as entidades principais a seguir.

## <a name="actions-preview"></a>Ações (visualização)

Executar uma ação imediata proteger contra ameaças usando a entidade [securityAction](securityaction.md)de Segurança do Microsoft Graph. Quando um analista de segurança descobre um indicador novo, como um arquivo mal-intencionado, URL, domínio ou endereço IP, a proteção pode ser habilitada instantaneamente em suas soluções de segurança da Microsoft. Usar uma ação específica do provedor, ver todas as ações executadas e cancelar uma ação, se necessário. Experimente ações de segurança com o [Microsoft Defender para Ponto de Extremidade](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) (antigo Microsoft Defender ATP) para bloquear atividades mal-intencionadas nos seus pontos de extremidade com Windows usando propriedades vistas em alertas ou identificadas durante as investigações.

  > **Observação:** Ações de segurança no momento apenas oferecem suporte às permissões do aplicativo.

## <a name="alerts"></a>Alertas

Os alertas são possíveis problemas de segurança no locatário de um cliente identificado pela Microsoft ou por soluções de segurança de parceiros identificados e sinalizados para ação ou notificação. Com a entidade de [alertas](alert.md) de Segurança do Microsoft Graph, é possível unificar e simplificar o gerenciamento dos problemas de segurança de todas as soluções integradas. Isso também permite que os aplicativos correlacionem alertas e contextos para melhorar a resposta e a proteção contra ameaças. Com o recurso de atualização de alertas, é possível sincronizar o status de alertas específicos em diferentes produtos e serviços de segurança que estão integrados à API de Segurança do Microsoft Graph atualizando sua entidade de [alertas](alert.md).

Alertas dos seguintes provedores estão disponíveis por meio da API de segurança do Microsoft Graph. O suporte para alertas GET, alertas PATCH e inscrições (via webhooks) é indicado na tabela a seguir.

| Provedor de segurança | <p align="center">Alerta GET</p>| <p align="center">Alerta PATCH</p>| <p align="center">Assinar o alerta</p>|
|:------------------|:---------|:-----------|:------------------|
|[Central de Segurança do Azure](/azure/security-center/security-center-alerts-type)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Proteção de identidade do Azure Active Directory](/azure/active-directory/identity-protection/playbook) | <p align="center">&#x2713;</p> | <p align="center">[Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
| [Microsoft Defender for Cloud Apps](/cloud-app-security/monitor-alerts) (antigo Microsoft Cloud App Security) | <p align="center">&#x2713;</p> | <p align="center">[Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Microsoft Defender para Ponto de Extremidade](/windows/security/threat-protection/microsoft-defender-atp/attack-simulations) (antigo Microsoft Defender ATP)**| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center"> [Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Microsoft Defender para Identidade](/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories) (antigo Azure Advanced Threat Protection)***| <p align="center">&#x2713;</p> | <p align="center">[Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|Microsoft 365 <ul><li> [Padrão](/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Segurança no Aplicativo na Nuvem](/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li><li>Alerta personalizado</li></ul> | <p align="center">&#x2713;</p> | <p align="center"> [Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Proteção de Informações do Azure](/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(visualização)**| <p align="center">&#x2713;</p> | <p align="center">[Problema de arquivo](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Azure Sentinel](/azure/sentinel/quickstart-get-visibility) **(visualização)**| <p align="center">&#x2713;</p> | <p align="center">Não possui suporte do Azure Sentinel </p> | <p align="center">&#x2713;</p> |
> **Observação:** Novos provedores estão se integrando continuamente ao ecossistema de Segurança do Microsoft Graph. Para requerer suporte aos novos provedores ou suporte estendido para os provedores existentes, [registre o problema no repositório GitHub de segurança do Microsoft Graph](https://github.com/microsoftgraph/security-api-solutions/issues/new).

\* Problema no arquivo: o status do alerta é atualizado nos aplicativos integrados da API de segurança do Microsoft Graph, mas não reflete na experiência de gerenciamento do provedor.

\*\* O Microsoft Defender para Ponto de Extremidade exige [funções de usuário](/windows/security/threat-protection/microsoft-defender-atp/user-roles) adicionais para aquelas requeridas pela API de Segurança do Microsoft Graph. Somente os usuários do Microsoft Defender para Ponto de Extremidade e as funções da API de Segurança do Microsoft Graph podem ter acesso aos dados do Microsoft Defender para Ponto de Extremidade. A autenticação somente para aplicativos não é limitada por isso. Portanto, recomendamos que você use um token de autenticação somente para aplicativos.

\*\*\* Os alertas do Microsoft Defender para Identidade estão disponíveis por meio da integração com o Microsoft Defender for Cloud Apps. Isso significa que você receberá alertas do Microsoft Defender para Identidade somente se tiver ingressado no portal Unified SecOps e conectado o Microsoft Defender para Identidade com o Microsoft Defender for Cloud Apps. Saiba mais sobre [como integrar o Microsoft Defender para Identidade com o Microsoft Defender for Cloud Apps.](/azure-advanced-threat-protection/atp-mcas-integration)

## <a name="attack-simulation-and-training-preview"></a>Simulação de ataque e treinamento (visualização)

[Simulação de ataque e treinamento](/microsoft-365/security/office-365-security/attack-simulation-training) é parte do [Microsoft Defender para Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true). Esse serviço permite que os usuários em um locatário experimentem um ataque de phishing benigno realista e aprendam com ele. Simulação de engenharia social e experiências de treinamento para usuários finais ajudam a reduzir o risco de usuários serem violados por meio dessas técnicas de ataque. A API de simulação e treinamento de ataque permite que os administradores de locatário visualizem os exercícios e treinamentos de [simulação](simulation.md) lançados e obtenham [relatórios](report-m365defender-reports-overview.md) sobre os insights derivados dos comportamentos online dos usuários nas simulações de phishing.

## <a name="ediscovery-preview"></a>Descoberta Eletrônica (versão prévia)

O [Microsoft Purview eDiscovery (Premium)](/microsoft-365/compliance/overview-ediscovery-20) fornece um fluxo de trabalho de ponta a ponta para preservar, coletar, analisar, revisar e exportar conteúdo que responde às investigações internas e externas de sua organização.

## <a name="information-protection"></a>Proteção de informações

**Etiquetas** - As Etiquetas de proteção de informações fornecem detalhes sobre como aplicar corretamente uma etiqueta de sensibilidade às informações. A API da etiquetas de proteção de informações descreve a configuração das etiquetas de sensibilidade que se aplicam a um usuário ou locatário.

**Avaliação de riscos** - A API de avaliação de ameaças do Microsoft Graph ajuda as organizações a avaliar a ameaça recebida por qualquer usuário em um locatário. Isso permite que os clientes denunciem spam ou emails suspeitos, URLs de phishing ou anexos de malware que receberem para a Microsoft. A Microsoft verifica o exemplo em questão e as políticas organizacionais em jogo antes de gerar um resultado para que os administradores de locatários possam entender o veredicto de verificação de ameaças e ajustar sua política organizacional. Eles também podem usá-lo para denunciar emails legítimos para evitar que sejam bloqueados.

> **Nota:** Recomendamos que você use a API de [submissão de ameaças](https://github.com/microsoftgraph/microsoft-graph-docs/pull/16242/files#threat-submission).

## <a name="secure-score"></a>Classificação de Segurança

A [Microsoft Secure Score](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358) é uma solução de análise da segurança que fornece visibilidade ao seu portfólio de segurança e mostra como melhorá-lo. Com uma única classificação, é possível entender melhor o que você fez para reduzir o risco em soluções da Microsoft. Você pode também comparar sua classificação com outras organizações e ver como tem sido a tendência ao longo do tempo. As entidades [secureScore](securescores.md) e [secureScoreControlProfile](securescorecontrolprofiles.md) de Segurança do Microsoft Graph ajudam a equilibrar a segurança e a produtividade de que sua organização precisa, além de habilitar o mix adequado de recursos de segurança. Você também pode projetar qual seria sua classificação depois de adotar recursos de segurança.

## <a name="threat-intelligence-indicators-preview"></a>Indicadores de inteligência contra ameaças (visualização)

Indicadores de ameaças, também conhecidos como indicadores de compromisso (IoCs), representam dados sobre ameaças conhecidas, como arquivos mal-intencionados, URLs, domínios e endereços IP. Os clientes podem gerar indicadores através da coleta interna de inteligência contra ameaças ou adquirir indicadores de comunidades de inteligência contra ameaças, feeds licenciados e outras fontes. Esses indicadores, em seguida, são usados nas várias ferramentas de segurança para proteger contra ameaças relacionadas.

A entidade de segurança do Microsoft Graph [tiIndicators](tiindicator.md) permite que os clientes alimentem os indicadores de ameaças nas soluções de segurança da Microsoft para habilitar ações em bloco e de alerta em atividades mal-intencionados ou permitir ações de supressão para determinados indicadores não relevantes para a organização. Quando você envia indicadores, a solução Microsoft que utilizará a indicação e a ação a ser tomada sobre o indicador são especificadas.

Você pode integrar a entidade [tiIndicator](tiindicator.md) em seu aplicativo ou use uma das seguintes plataformas integradas de inteligência contra ameaças (DICA):

- [Compartilhamento de inteligência contra Ameaças Palo Alto Networks](https://www.paloaltonetworks.com/products/secure-the-network/subscriptions/minemeld)
- [Plataforma de inteligência contra ameaças de Código Aberto MISP](http://www.misp-project.org/) disponíveis em [exemplo IT](https://aka.ms/tipmispsample)

Os indicadores de ameaças enviados por meio da API de Segurança do Microsoft Graph estão disponíveis hoje nos seguintes produtos:

- [Azure Sentinel](/azure/sentinel/overview) – Permite correlacionar indicadores de ameaças com dados de log para receber alertas de atividades mal-intencionadas.
- [Microsoft Defender para Ponto de Extremidade](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection): permite que você alerte e/ou bloqueie os indicadores de ameaças associados a atividades mal-intencionadas. Você também pode permitir que um indicador ignore o indicador das investigações automatizadas. Para mais detalhes sobre os tipos de indicadores com suporte e limites de contagens de indicadores por locatário, confira [Gerenciar indicadores](/windows/security/threat-protection/microsoft-defender-atp/manage-indicators).

O suporte a outros serviços de segurança da Microsoft estará disponível em breve.

## <a name="threat-submission"></a>Envio de ameaça

A API de envio de ameaças do Microsoft Graph ajuda as organizações a enviar uma ameaça recebida por qualquer usuário em um locatário. Isso permite que os clientes denunciem spam ou emails suspeitos, URLs de phishing ou anexos de malware que receberem para a Microsoft. A Microsoft verifica o envio em relação às políticas organizacionais em vigor e o envia para avaliadores humanos para análise. O resultado ajuda os administradores de locatários a entender o veredicto de verificação de ameaças e ajustar sua política organizacional. Os administradores também podem usar os resultados para relatar emails legítimos para evitar que sejam bloqueados.

> **Nota: ** Recomendamos que você use essa API em vez da API de avaliação de ameaças de proteção de informações obsoleta. A API de envio de ameaças fornece funcionalidade unificada de envio de ameaças de segurança e adiciona suporte a resultados unificados, suporte a consultas de envio de usuários, suporte a lista de bloqueio de permissão de locatário, suporte a revisão de administrador e suporte ao modo somente aplicativo.

## <a name="common-use-cases"></a>Casos de uso comuns

A seguir, há algumas das solicitações mais populares para trabalhar com a API de Segurança do Microsoft Graph.

| **Casos de uso**   | **Recursos REST** | **Experimentar no Explorador do Graph** |
|:---------------|:--------|:----------|
| **Ações (visualização)**|||
| Obter ações de segurança | [Obter ações de segurança](../api/securityaction-get.md)|[https://graph.microsoft.com/beta/security/securityActions/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Listar ações de segurança| [Listar ações de segurança](../api/securityactions-list.md)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Criar ações de segurança|[Criar ações de segurança](../api/securityactions-post.md)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Cancelar ações de segurança|[Cancelar ações de segurança](../api/securityaction-cancelsecurityaction.md)| [https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}/cancelSecurityAction&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
| **Alertas**|||
| Listar alertas | [List alerts](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| Atualizar alertas | [Atualizar alertas](../api/alert-update.md) </br> [Atualizar vários alertas](../api/alert-updatealerts.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) </br> [https://graph.microsoft.com/beta/security/alerts/updateAlerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/updateAlerts&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
| **Simulação de ataque e treinamento (visualização)**|||
|Listar simulações|[Listar simulações](../api/attacksimulationroot-list-simulations.md)|[https://graph.microsoft.com/beta/security/attackSimulation/simulations](https://developer.microsoft.com/graph/graph-explorer?request=security/attackSimulation/simulations&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Obter o relatório de visão geral da simulação|[Obter o relatório de visão geral da simulação](../api/simulationreportoverview-get.md)|[https://graph.microsoft.com/beta/security/attackSimulation/simulations/{id}/report/overview](https://developer.microsoft.com/graph/graph-explorer?request=security/attackSimulation/simulations/{id}/report/overview&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Listar os relatório dos usuários de simulação|[Listar os relatório dos usuários de simulação](../api/usersimulationdetails-list.md)|[https://graph.microsoft.com/beta/security/attackSimulation/simulations/{id}/report/simulationUsers](https://developer.microsoft.com/graph/graph-explorer?request=security/attackSimulation/simulations/{id}/report/simulationUsers&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
| **Descoberta eletrônica**|||
|Listar casos de Descoberta Eletrônica|[Listar eDiscoveryCases](../api/security-casesroot-list-ediscoverycases.md)|[https://graph.microsoft.com/beta/security/cases/eDiscoveryCases](https://developer.microsoft.com/graph/graph-explorer?request=security%2Fcases%2FeDiscoverycases&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Listar operações de caso de Descoberta Eletrônica|[Listar caseOperations](../api/security-ediscoverycase-list-operations.md)|[https://graph.microsoft.com/beta/security/cases/eDiscoverycases/{id}/operations](https://developer.microsoft.com/graph/graph-explorer?request=security%2Fcases%2FeDiscoverycases%2F%7Bid%7D%2Foperations&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
| **Classificações de segurança**|||
|Listar classificações de segurança|[Listar secureScores](../api/securescores-list.md)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
| **Perfis de controle da classificação de segurança**|||
|Listar perfis de controle da classificação de segurança|[Listar secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Atualizar perfis de controle da classificação de segurança|[Atualizar secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|
| **Indicações de inteligência contra ameaças (visualização)**|||
|Obter o indicador TI|[Obter tiIndicator](../api/tiindicator-get.md)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Listar Indicadores TI | [Listar tiIndicators](../api/tiindicators-list.md) | [https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Criar um Indicadores TI|[Criar tiIndicator](../api/tiindicators-post.md)|[https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Enviar Indicadores TI|[Enviar tiIndicators](../api/tiindicator-submittiindicators.md)| [https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/submitTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
|Atualizar Indicadores TI|[Atualizar tiIndicator](../api/tiindicator-update.md) </br>[Atualizar vários tiIndicators](../api/tiindicator-updatetiindicators.md)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) </br>[https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/updateTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Excluir Indicadores TI|[Excluir tiIndicator](../api/tiindicator-delete.md) </br>[Excluir vários tiIndicators](../api/tiindicator-deletetiindicators.md) </br>[Excluir tiIndicator por externalId](../api/tiindicator-deletetiindicatorsbyexternalid.md)| EXCLUIR </br>[https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=DELETE&version=beta&GraphUrl=https://graph.microsoft.com) </br>POSTAR</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)</br>POSTAR</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicatorsByExternalId&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
| **Envio de ameaça**|||
|Receba o envio de ameaças por email|[Obter emailThreat](../api/security-emailthreatsubmission-get.md)| [https://graph.microsoft.com/beta/security/threatSubmission/emailThreats/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/emailThreats/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Listar envios de ameaças por email | [Listar emailThreats](../api/security-emailthreatsubmission-list.md) | [https://graph.microsoft.com/beta/threatSubmission/emailThreats](https://developer.microsoft.com/graph/graph-explorer?request=threatSubmission/emailThreats&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Criar envio de ameaças de email|[Crar emailThreat](../api/security-emailthreatsubmission-post-emailthreats.md)|[https://graph.microsoft.com/beta/security/threatSubmission/emailThreats](https://developer.microsoft.com/graph/graph-explorer?request=security/security/threatSubmission/emailThreats&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Revisar o envio de ameaças por email|[Revisar emailThreat](../api/security-emailthreatsubmission-review.md)|[https://graph.microsoft.com/beta/security/threatSubmission/emailThreats/{id}/review](https://developer.microsoft.com/graph/graph-explorer?request=security/security/threatSubmission//emailThreats/{id}/review&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Obter envio de ameaça de arquivo|[Obter fileThreat](../api/security-filethreatsubmission-get.md)| [https://graph.microsoft.com/beta/security/threatSubmission/fileThreats/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/urlThreats/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Listar envios de ameaças de arquivo | [Listar fileThreats](../api/security-filethreatsubmission-list.md) | [https://graph.microsoft.com/beta/threatSubmission/urlThreats](https://developer.microsoft.com/graph/graph-explorer?request=threatSubmission/fileThreats&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Criar envio de ameaças de arquivo|[Criar fileThreat](../api/security-filethreatsubmission-post-fileThreats.md)|[https://graph.microsoft.com/beta/security/threatSubmission/fileThreats](https://developer.microsoft.com/graph/graph-explorer?request=security/security/threatSubmission/fileThreats&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Obter envio de ameaça de URL|[Obter urlThreat](../api/security-urlthreatsubmission-get.md)| [https://graph.microsoft.com/beta/security/threatSubmission/urlThreats/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/urlThreats/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Listar envios de ameaças à URL | [Listar urlThreats](../api/security-urlthreatsubmission-list.md) | [https://graph.microsoft.com/beta/security/threatSubmission/urlThreats](https://developer.microsoft.com/graph/graph-explorer?request=threatSubmission/urlThreats&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Criar envio de ameaça de URL|[Criar urlThreat](../api/security-urlthreatsubmission-post-urlthreats.md)|[https://graph.microsoft.com/beta/security/threatSubmission/urlThreats](https://developer.microsoft.com/graph/graph-explorer?request=security/security/threatSubmission/urlThreats&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Obter política de envio de ameaças por email|[Obter emailThreatSubmissionPolicy](../api/security-emailthreatsubmission-get.md)| [https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/emailThreatSubmissionPolicies/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Listar políticas de envio de ameaças por email | [Listar emailThreatSubmissionPolicies](../api/security-emailthreatsubmissionpolicy-list.md) | [https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/emailThreatSubmissionPolicies&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Criar política de envio de ameaças por email|[Criar emailThreatSubmissionPolicy](../api/security-emailthreatsubmission-post-emailthreats.md)|[https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies](https://developer.microsoft.com/graph/graph-explorer?request=/security/threatSubmission/emailThreats&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Atualizar a política de envio de ameaças por email|[Atualizar emailThreatSubmissionPolicy](../api/security-emailthreatsubmission-post-emailthreats.md)|[https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/security/threatSubmission/emailThreatSubmissionPolicies/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|
|Excluir política de envio de ameaças por email|[Excluir emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-delete.md)|[https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/threatSubmission/emailThreatSubmissionPolicies/{id}&method=DELETE&version=beta&GraphUrl=https://graph.microsoft.com)|

Você pode usar o Microsoft Graph [webhooks](/graph/webhooks) para assinar e receber notificações sobre as atualizações de entidades de Segurança do Microsoft Graph.

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para esses conjuntos de API.

## <a name="next-steps"></a>Próximas etapas

A API de Segurança do Microsoft Graph pode abrir novas formas para você interagir com diferentes soluções de segurança da Microsoft e de parceiros. Siga estas etapas para começar:

- Analise [alerts](alert.md), [tiIndicator](tiindicator.md) (preview), [securityAction](securityaction.md) (preview), [secureScore](securescores.md) e [secureScoreControlProfiles](securescorecontrolprofiles.md).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer). Em **Consultas de Exemplo**, escolha **mostrar mais amostras** e defina a categoria Segurança como **on**.
- Experimente [assinar e receber notificações](/graph/webhooks) sobre alterações de entidade.

Precisa de mais ideias? Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/partners).

## <a name="see-also"></a>Confira também

[Codifique e contribua](https://github.com/microsoftgraph/security-api-solutions/blob/master/CONTRIBUTING.md) com esses exemplos da API de Segurança do Microsoft Graph:

- [Amostra do ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Amostra do Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Amostra do Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)
- [Exemplo do PowerShell](https://aka.ms/graphsecuritypowershellsample)
- [Outros exemplos ou contribuir com um novo exemplo](https://aka.ms/graphsecurityapicode)

Explore outras opções para se conectar com a API de segurança da Microsoft Graph:

- [Conectores de Segurança do Microsoft Graph para Aplicativos de Lógica, Flow e PowerApps](/azure/connectors/connectors-integrate-security-operations-create-api-microsoft-graph-security)
- [Exemplos de bloco de anotações Jupyter](https://aka.ms/graphsecurityjupyternotebooks)

Participe da comunidade:

- [Junte-se à comunidade técnica](https://techcommunity.microsoft.com/t5/microsoft-graph-security-api/bd-p/SecurityGraphAPI)
- [Discussão no StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)