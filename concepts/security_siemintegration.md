# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Integre os alertas da API de segurança do Microsoft Graph com um SIEM

A API de segurança do Microsoft Graph permite gerenciar alertas de segurança de todos os produtos de segurança da Microsoft, conhecidos como provedores de segurança do Microsoft Graph, por meio de um único ponto de extremidade REST. Algumas organizações já ingerem dados de log específicos do Azure por meio do Monitor do Azure em soluções SIEM. Para simplificar a integração, os alertas de segurança disponíveis por meio da API de segurança do Microsoft Graph também podem ser provisionados pelo cliente para a assinatura por meio do Monitor do Azure. Se a sua organização já configurou a integração do Monitor do Azure com a sua solução SIEM, você já pode receber facilmente o fluxo de alertas de segurança da sua organização, além dos seus dados existentes disponíveis por meio do Monitor do Azure.

O Monitor do Azure é compatível com conectores para vários produtos SIEM. Para obter uma lista dos produtos SIEM compatíveis, consulte [Enviar dados de monitoramento a um hub de evento](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub). A Integração com a API de segurança do Microsoft Graph está disponível atualmente para [Splunk](https://splunkbase.splunk.com/) e [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem).

Para obter informações sobre a integração da API de segurança do Microsoft Graph para soluções SIEM específicas, consulte:

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
