---
title: Integrar alertas da API de Segurança do Microsoft Graph com um SIEM
description: A API de Segurança do Microsoft Graph permite o gerenciamento de alertas de segurança de todos os produtos de segurança da Microsoft, conhecidos como provedores de Segurança do Microsoft Graph, por meio de um ponto de extremidade REST único. Talvez algumas organizações já incluam dados de log específicos do Azure por meio do Azure Monitor em soluções do SIEM. Para simplificar a integração, os alertas de segurança disponíveis por meio da API de Segurança do Microsoft Graph também possam ser provisionados pelo cliente para sua assinatura por meio do Azure Monitor. Se a organização já tiver configurado a integração do Azure Monitor com sua solução do SIEM, você já poderá transmitir facilmente os alertas de segurança da organização, além dos dados existentes disponíveis, pelo Azure Monitor.
ms.openlocfilehash: ca2952163ab8894cae4c22f726b45b1be94a8b1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091639"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Integrar alertas da API de Segurança do Microsoft Graph com um SIEM

A API de Segurança do Microsoft Graph permite o gerenciamento de alertas de segurança de todos os produtos de segurança da Microsoft, conhecidos como provedores de Segurança do Microsoft Graph, por meio de um ponto de extremidade REST único. Talvez algumas organizações já incluam dados de log específicos do Azure por meio do Azure Monitor em soluções do SIEM. Para simplificar a integração, os alertas de segurança disponíveis por meio da API de Segurança do Microsoft Graph também possam ser provisionados pelo cliente para sua assinatura por meio do Azure Monitor. Se a organização já tiver configurado a integração do Azure Monitor com sua solução do SIEM, você já poderá transmitir facilmente os alertas de segurança da organização, além dos dados existentes disponíveis, pelo Azure Monitor.

O Azure Monitor é compatível com conectores para vários produtos SIEM. Para obter uma lista de produtos SIEM com suporte, confira [enviar dados de monitoramento para um hub de eventos](https://docs.microsoft.com/pt-BR/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). A integração da API de Segurança do Microsoft Graph está disponível para [Splunk](https://splunkbase.splunk.com/) e [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem).

Para saber sobre a integração da API de Segurança do Microsoft Graph para soluções SIEM específicas, confira:

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
