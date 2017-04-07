# <a name="subscribedsku-resource-type"></a>Tipo de recurso subscribedSku

Contém informações sobre um serviço SKU assinado por uma empresa.

Somente a operação de leitura tem nos SKUs inscritos; criar, atualizar e excluir não têm suporte. Não há suporte para expressões de filtro de consulta.

Herda de [directoryObject](directoryobject.md).


## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get subscribedSku](../api/subscribedsku_get.md) | [subscribedSku](subscribedsku.md) |Ler propriedades do objeto subscribedSku.|

## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|capabilityStatus|Cadeia de caracteres|Por exemplo, "Ativado", "Bloqueado" e "Suspenso".|
|consumedUnits|Int32|O número de licenças que foram atribuídas.|
|id|String|O identificador exclusivo do objeto SKU assinado. Chave. Somente leitura.|
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)|Informações sobre o número e o status das licenças pré-pagas.|
|servicePlans|Coleção [servicePlanInfo](serviceplaninfo.md)|Informações sobre os planos do serviço que estão disponíveis com o SKU.|
|skuId|Guid|O identificador exclusivo (GUID) do SKU do serviço.|
|skuPartNumber|String|O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".|
|appliesTo|Cadeia de caracteres|Por exemplo, “Usuário” ou “Empresa”.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
