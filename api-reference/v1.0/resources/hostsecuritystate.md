# <a name="hostsecuritystate-resource-type"></a>tipo de recurso hostSecurityState

Contém informações com estado sobre o host (incluindo dispositivos, computadores e assim por diante).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|fqdn|Cadeia de caracteres|FQDN do host (nome de domínio totalmente qualificado) (por exemplo, `machine.company.com`).|
|isAzureAadJoined|Booleano|Verdadeiro se o host estiver associado aos serviços de domínio do Active Directory do Azure.|
|isAzureAadRegistered|Booleano|Verdadeiro se o host estiver registrado no Registro de Dispositivos do Active Directory do Azure (dispositivos BYOD - ou seja, não totalmente gerenciados pela empresa).|
|isHybridAzureDomainJoined|Booleano|Verdadeiro se o host estiver associado a um domínio do Active Directory local.|
|netBiosName|Cadeia de caracteres|O nome do host local, sem o nome de domínio DNS.|
|os|Cadeia de caracteres|Sistema operacional do host. (Por exemplo, Windows10, MacOS, RHEL, etc.).|
|privateIpAddress|Cadeia de caracteres|Endereço particular IPv4 ou IPv6 (não roteável) (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.|
|publicIpAddress|Cadeia de caracteres|Endereço IPv4 ou IPv6 publicamente roteável (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.|
|riskScore|Cadeia de caracteres|Pontuação de risco do host gerada/calculada pelo provedor.  Intervalo de valor recomendado de 0-1, que equivale a um percentual.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
