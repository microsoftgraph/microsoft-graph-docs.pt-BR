---
title: tipo de recurso de synchronizationTemplate
description: " qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o esquema de sincronização."
localization_priority: Normal
ms.openlocfilehash: 75df13d55cfb58aafe8a751279e103424aa29367
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516550"
---
# <a name="synchronizationtemplate-resource-type"></a>tipo de recurso de synchronizationTemplate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece configurações de sincronização pré-configurado para um determinado aplicativo. Essas configurações serão usadas por padrão para qualquer [trabalho de sincronização](synchronization-synchronizationjob.md) que baseia-se no modelo. O desenvolvedor do aplicativo especifica o modelo; qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o [esquema de sincronização](synchronization-synchronizationschema.md).

Você pode fornecer vários modelos para um aplicativo e designar um modelo padrão. Se vários modelos estão disponíveis para o aplicativo que você está interessado, seek orientação específica de aplicativos para determinar qual deles melhor atenda às suas necessidades.

## <a name="methods"></a>Métodos

| Método        | Tipo de retorno               | Descrição                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |coleção [synchronizationTemplate](synchronization-synchronizationtemplate.md)  |Lista os modelos disponíveis para um aplicativo ou uma instância de aplicativo (entidade de serviço).|
|[Get](../api/synchronization-synchronizationtemplate-get.md)      |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Leia as propriedades e relações do objeto **synchronizationTemplate** .|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                      | Descrição                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |String                     |Identificador exclusivo do modelo.|
|ApplicationId  |Cadeia de caracteres                     |Identificador do aplicativo que pertence este modelo.|
|Padrão.        |Booliano                    |`true`Se esse modelo é recomendado para ser o padrão para o aplicativo.|
|description    |String                     |Descrição do modelo.|
|detectáveis   |String                     |`true`Se este modelo deve aparecer na coleção de modelos disponíveis para a instância do aplicativo (entidade de serviço).|
|factoryTag     |String                     |Uma das marcas de fábrica conhecido suportadas pelo mecanismo de sincronização. O **factoryTag** informa ao mecanismo de sincronização qual implementação usar durante o processamento de trabalhos com base nesse modelo.|
|Metadata       |coleção metadataEntry   |Propriedades adicionais de extensão. A menos que mencionado explicitamente, valores de metadados não devem ser alterados.|

## <a name="relationships"></a>Relacionamento
| Relação      | Tipo      |Descrição|
|:------------------|:----------|:----------|
|SCHEMA             |[synchronizationSchema](synchronization-synchronizationschema.md)     |Esquema de sincronização padrão para os trabalhos baseados nesse modelo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}-->

```json
{
  "applicationId": "String (identifier)",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "id": "String (identifier)",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "schema": {"@odata.type": "microsoft.graph.synchronizationSchema"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
