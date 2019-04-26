---
title: Integrar alertas da API de Segurança do Microsoft Graph com um SIEM
description: A API de Segurança do Microsoft Graph permite o gerenciamento de alertas de segurança de todos os produtos de segurança da Microsoft, conhecidos como provedores de Segurança do Microsoft Graph, por meio de um ponto de extremidade REST único. Talvez algumas organizações já incluam dados de log específicos do Azure por meio do Azure Monitor em soluções do SIEM. Para simplificar a integração, os alertas de segurança disponíveis por meio da API de Segurança do Microsoft Graph também possam ser provisionados pelo cliente para sua assinatura por meio do Azure Monitor. Se a organização já tiver configurado a integração do Azure Monitor com sua solução do SIEM, você já poderá transmitir facilmente os alertas de segurança da organização, além dos dados existentes disponíveis, pelo Azure Monitor.
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 92a5416f68ccbc6fbbd0001c473f1daf2fe21187
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556926"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Integrar alertas da API de Segurança do Microsoft Graph com um SIEM

A API de Segurança do Microsoft Graph permite o gerenciamento de alertas de segurança de todos os produtos de segurança da Microsoft, conhecidos como provedores de Segurança do Microsoft Graph, por meio de um ponto de extremidade REST único. Talvez algumas organizações já incluam dados de log específicos do Azure por meio do Azure Monitor em soluções do SIEM. Para simplificar a integração, os alertas de segurança disponíveis por meio da API de Segurança do Microsoft Graph também possam ser provisionados pelo cliente para sua assinatura por meio do Azure Monitor. Se a organização já tiver configurado a integração do Azure Monitor com sua solução do SIEM, você já poderá transmitir facilmente os alertas de segurança da organização, além dos dados existentes disponíveis, pelo Azure Monitor.

Os alertas dos seguintes provedores de segurança estão disponíveis por meio da integração de SIEM:

- [Central de Segurança do Azure](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Proteção de identidade do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Segurança no Aplicativo da Nuvem da Microsoft](https://docs.microsoft.com/cloud-app-security/monitor-alerts)
- [Proteção de Informações do Azure](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(visualização)**
- [Proteção Avançada contra Ameaças do Azure](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories) **(versão prévia)**
- [Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility) **(versão prévia)**

O Azure Monitor é compatível com conectores para vários produtos SIEM. Para obter uma lista de produtos SIEM com suporte, confira [enviar dados de monitoramento para um hub de eventos](https://docs.microsoft.com/pt-BR/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). A integração da API de Segurança do Microsoft Graph está disponível para [Splunk](https://splunkbase.splunk.com/) e [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem).

Para saber sobre a integração da API de Segurança do Microsoft Graph para soluções SIEM específicas, confira:

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
