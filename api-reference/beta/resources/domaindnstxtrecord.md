# Tipo de recurso domainDnsTxtRecord
<a id="domaindnstxtrecord-resource-type" class="xliff"></a>

Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).

## Métodos
<a id="methods" class="xliff"></a>
Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.

## Propriedades
<a id="properties" class="xliff"></a>
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura. |
|isOptional|Booliano| Se for falso, o registro TXT deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio. |
|rótulo|String| O valor a ser usado ao configurar a propriedade *name* do registro TXT no host DNS.|
|recordType|String| Tipo do registro DNS. Este valor sempre será *Txt*. Chave |
|supportedService|String| O Microsoft Online Services ou o recurso que tiver uma dependência neste registro TXT.</br></br>Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|text|String| O valor usado ao configurar a propriedade *text* no host DNS. |
|ttl|Int32| O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro MX no host DNS. Não anulável |

## Relações
<a id="relationships" class="xliff"></a>
Nenhum


## Representação JSON
<a id="json-representation" class="xliff"></a>
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->