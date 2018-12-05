---
title: Integre os alertas de API de segurança do Microsoft Graph um SIEM
description: A API de segurança do Microsoft Graph permite gerenciar alertas de segurança de todos os produtos de segurança da Microsoft, conhecidos como provedores de segurança do Microsoft Graph, por meio de um único ponto de extremidade do REST. Algumas organizações já podem incluir os dados de log específicos do Azure por meio do Monitor do Windows Azure em soluções SIEM. Para simplificar a integração, os alertas de segurança disponíveis por meio da API de segurança do Microsoft Graph podem ser fornecidos pelo cliente para a assinatura por meio do Monitor do Windows Azure. Se sua organização já tiver configurado a integração do Windows Azure Monitor com sua solução SIEM, você pode agora transmitir facilmente o alertas de segurança da sua organização além dos seus dados existentes disponíveis por meio do Monitor do Windows Azure.
ms.openlocfilehash: ca2952163ab8894cae4c22f726b45b1be94a8b1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091639"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Integre os alertas de API de segurança do Microsoft Graph um SIEM

A API de segurança do Microsoft Graph permite gerenciar alertas de segurança de todos os produtos de segurança da Microsoft, conhecidos como provedores de segurança do Microsoft Graph, por meio de um único ponto de extremidade do REST. Algumas organizações já podem incluir os dados de log específicos do Azure por meio do Monitor do Windows Azure em soluções SIEM. Para simplificar a integração, os alertas de segurança disponíveis por meio da API de segurança do Microsoft Graph podem ser fornecidos pelo cliente para a assinatura por meio do Monitor do Windows Azure. Se sua organização já tiver configurado a integração do Windows Azure Monitor com sua solução SIEM, você pode agora transmitir facilmente o alertas de segurança da sua organização além dos seus dados existentes disponíveis por meio do Monitor do Windows Azure.

Monitor Azure suporta conectores para vários produtos SIEM. Para obter uma lista dos produtos SIEM suportados, consulte [Enviar dados a um hub de evento de monitoramento](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). Integração de API de segurança do Microsoft Graph está disponível atualmente para [Splunk](https://splunkbase.splunk.com/) e [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem).

Para obter informações sobre a integração de API de segurança do Microsoft Graph para soluções SIEM específicas, consulte:

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
