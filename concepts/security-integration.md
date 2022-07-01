---
title: Integração das soluções de segurança usando a API de segurança do Microsoft Graph
description: Use essas opções para se conectar com o Microsoft Graph API de Segurança e trabalhar com dados em um formato unificado entre provedores de segurança de parceiros e da Microsoft com suporte.
author: preetikr
ms.localizationpriority: high
ms.prod: security
ms.openlocfilehash: c221192e91d357c442dfd3eaa8ad32ae1685358e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437545"
---
# <a name="security-solution-integrations-using-the-microsoft-graph-security-api"></a>Integração das soluções de segurança usando a API de segurança do Microsoft Graph

Você pode se conectar à API de segurança do Microsoft Graph usando qualquer uma das opções a seguir. Essas opções permitem que você trabalhe com dados em um formato unificado entre [os provedores de segurança da Microsoft e parceiros com suporte](/graph/api/resources/security-api-overview#alerts) por meio de uma única integração:

- **Utilize as opções de integração suportadas:** Consulte a [lista de opções de integração suportadas](./security-concept-overview.md#why-use-the-microsoft-graph-security-api) tais como escrever código para conectar diretamente sua aplicação para obter ideias ricas. Use [exemplos](https://aka.ms/graphsecurityapicode) para começar.
- **Utilize as integrações nativas e conectores construídos por parceiros Microsoft:** Consulte as [soluções parceiras Microsoft Graph Security API](https://aka.ms/graphsecuritypartnerships) para usar essas integrações.  
- **Use conectores criados pela Microsoft:** Confira a [lista de conectores](#list-of-connectors-from-microsoft) que você pode usar para se conectar com a API por meio de uma variedade de soluções para o gerenciamento de incidentes e segurança (SIEM), resposta de segurança e Orquestração (SOAR), acompanhamento de incidentes e gerenciamento de serviços (ITSM), relatórios e assim por diante.  

## <a name="list-of-connectors-from-microsoft"></a>Lista de conectores da Microsoft

| Tipo de solução | Nome | Conector | Comunicado |
|:-----|:--------|:--------|:----------|
| SIEM |Splunk Enterprise e Splunk Cloud|[Visão geral da API de Segurança do Microsoft Graph](https://aka.ms/graphsecuritysplunkaddon) | [Postagem no blog](https://aka.ms/graphsecuritysplunkaddonblogpost)<br>[Postagem no blog Splunk na nuvem](https://aka.ms/graphsecuritysplunkcloudblogpost)|
| SIEM |QRadar|[Protocolo da API de Segurança do Microsoft Graph e DSMs QRadas suportados](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/com.ibm.dsm.doc/c_logsource_Microsoft_Graph_Security_protocol.html)| - |
| ITSM |ServiceNow|[Integração de ingestão de alertas da API de Segurança do Microsoft Graph](https://docs.servicenow.com/bundle/orlando-security-management/page/product/secops-integration-sir/secops-integration-ms-graph/concept/ms-graph-about.html)| - |
| SOAR | Aplicativos lógicos do Azure/fluxo da Microsoft | [Conector de Segurança do Microsoft Graph para Aplicativos Lógicos do Azure, Aplicativos de Fluxo e Microsoft Flow](/azure/connectors/connectors-integrate-security-operations-create-api-microsoft-graph-security) | [Postagem no blog](https://aka.ms/graphsecurityconnectorsblogpost) |
| Automação | Módulo do PowerShell | [Módulo do PowerShell de segurança do Microsoft Graph](https://aka.ms/graphsecuritypowershellmodule) | [Postagem no blog](https://aka.ms/graphsecuritypowershellmodulepost) |
| Relatório | Power BI | [Conector de segurança do Microsoft Graph para Power BI](/power-bi/connect-data/desktop-connect-graph-security) | [Postagem no blog](https://aka.ms/graphsecuritypowerbiconnectorblogpost) |

Se você gostaria de apoiar integrações nativas em sua solução ou ser um fornecedor de dados para a API de segurança gráfica da Microsoft, analise as [oportunidades de parceria](./security-partner-overview.md).
