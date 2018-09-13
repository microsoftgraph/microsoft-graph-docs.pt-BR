# <a name="securityvendorinformation-resource-type"></a>tipo de recurso securityVendorInformation

Contém detalhes sobre o fornecedor, provedor e subprovedor de produtos/serviços de segurança (por exemplo,  vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|provider *|Cadeia de caracteres|Provedor específico (produto/serviço - não a empresa fornecedora); por exemplo, WindowsDefenderATP.|
|providerVersion|Cadeia de caracteres|Versão do provedor ou subprovidor, se ela existir, que gerou o alerta.|
|subProvider|Cadeia de caracteres|Subprovidor específico (sob o provedor agregador); por exemplo, WindowsDefenderATP.SmartScreen.|
|vendor *|Cadeia de caracteres|Nome do fornecedor de alertas (por exemplo, Microsoft, Dell, FireEye).|
(\* Indica um campo obrigatório.)

## <a name="json-representation"></a>Representação JSON

A seguir, uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
