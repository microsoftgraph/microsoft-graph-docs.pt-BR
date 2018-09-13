# <a name="networkconnection-resource-type"></a>tipo de recurso networkConnection

Contém informações com estado sobre a conexão de rede relacionada ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|applicationName|Cadeia de caracteres|Nome do aplicativo que gerencia a conexão de rede (por exemplo, Facebook, SMTP, etc.).|
|destinationAddress|Cadeia de caracteres|Endereço IP de destino (da conexão de rede).|
|destinationDomain|Cadeia de caracteres|Parte do domínio de destino da URL de destino. (por exemplo 'www.contoso.com').|
|destinationPort|Cadeia de caracteres|Porta de destino (da conexão de rede).|
|destinationUrl|Cadeia de caracteres|Cadeia de caracteres de URL/URI de conexão de rede - excluindo parâmetros. (por exemplo, 'www.contoso.com/products/default.html')|
|direção|connectionDirection|Direção da conexão de rede. Os valores possíveis são: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Data quando o domínio de destino foi registrado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|localDnsName|Cadeia de caracteres|A resolução do nome DNS local como aparece no cache DNS local do host (por exemplo, caso o arquivo 'hosts' tenha sido adulterado).|
|natDestinationAddress|Cadeia de caracteres|Endereço IP de destino da Conversão de Endereços de Rede.|
|natDestinationPort|Cadeia de caracteres|Porta de destino de Conversão de Endereços de Rede.|
|natSourceAddress|Cadeia de caracteres|Endereço IP de origem de conversão de endereço de rede.|
|natSourcePort|Cadeia de caracteres|Porta de origem da Conversão de Endereços de Rede.|
|protocolo|[securityNetworkProtocol](securitynetworkprotocol.md)|Protocolo de Rede. Os valores possíveis são: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|Cadeia de caracteres|Pontuação de risco gerada/calculada pelo provedor da conexão de rede. Intervalo de valor recomendado de 0-1, que equivale a um percentual.|
|sourceAddress|Cadeia de caracteres|Endereço IP de origem (da conexão de rede).|
|sourcePort|Cadeia de caracteres|Porta do IP de origem (da conexão de rede).|
|status|connectionStatus|Status da conexão de rede. Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|Cadeia de caracteres|Parâmetros (sufixo) da URL de destino.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkConnection"
}-->

```json
{
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "@odata.type: microsoft.graph.connectionDirection",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "@odata.type: microsoft.graph.connectionStatus",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->