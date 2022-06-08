---
título: "tipo de recurso siteSource": ""O contêiner de um site associado a um custodiante".
author: "SeunginLyu" ms.localizationpriority: medium ms.prod: "ediscovery" doc_type: resourcePageType
---

# <a name="sitesource-resource-type"></a>Tipo de recurso siteSource

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
O contêiner de um site associado a um guardião.

IInherits de [dataSource](../resources/security-datasource.md).


## <a name="methods"></a>Métodos
Nenhum.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|O usuário que criou **o siteSource**.|
|createdDateTime|DateTimeOffset|A data e a hora em **que o siteSource** foi criado.|
|displayName|String|O nome de exibição **do siteSource**. Esse será o nome do site do SharePoint.|
|id|Cadeia de caracteres| A ID do **siteSource**. A origem do site pode ser recuperada a qualquer momento com [Get site](../api/site-get.md) - https://graph.microsoft.com/v1.0/sites/{siteId}|
|holdStatus|String|O status de retenção do **siteSource**. Os valores possíveis são: `notApplied`, `applied`, `applying`, , `removing``partial`|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|site|[site](../resources/site.md)|O site do SharePoint associado ao **siteSource**.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.siteSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.siteSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

