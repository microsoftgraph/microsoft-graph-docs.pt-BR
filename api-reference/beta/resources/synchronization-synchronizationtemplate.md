---
title: tipo de recurso synchronizationtemplate
description: " qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o esquema de sincronização."
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9952b06276efa712068091ecd8b7b5dc5e6769d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520013"
---
# <a name="synchronizationtemplate-resource-type"></a>tipo de recurso synchronizationtemplate

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece configurações de sincronização pré-configuradas para um aplicativo específico. Essas configurações serão usadas por padrão para qualquer [trabalho de sincronização](synchronization-synchronizationjob.md) baseado no modelo. O desenvolvedor do aplicativo especifica o modelo; qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o [esquema de sincronização](synchronization-synchronizationschema.md).

Você pode fornecer vários modelos para um aplicativo e designar um modelo padrão. Se vários modelos estiverem disponíveis para o aplicativo em que você está interessado, procure orientação específica do aplicativo para determinar qual deles atende melhor às suas necessidades.

## <a name="methods"></a>Métodos

| Método        | Tipo de retorno               | Descrição                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |coleção [synchronizationtemplate](synchronization-synchronizationtemplate.md)  |Lista os modelos disponíveis para uma instância de aplicativo ou aplicativo (entidade de serviço).|
|[Get](../api/synchronization-synchronizationtemplate-get.md)      |[synchronizationtemplate](synchronization-synchronizationtemplate.md)   |Leia as propriedades e as relações do objeto **synchronizationtemplate** .|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                      | Descrição                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |Cadeia de caracteres                     |Identificador de modelo exclusivo.|
|ApplicationId  |Cadeia de caracteres                     |Identificador do aplicativo ao qual este modelo pertence.|
|Padrão.        |Boolean                    |`true`Se este modelo é recomendado para ser o padrão para o aplicativo.|
|description    |String                     |Descrição do modelo.|
|detectáveis   |String                     |`true`Se esse modelo deve aparecer na coleção de modelos disponíveis para a instância do aplicativo (entidade de serviço).|
|factoryTag     |String                     |Uma das marcas de fábrica conhecidas suportadas pelo mecanismo de sincronização. O **factoryTag** informa ao mecanismo de sincronização que implementação usar ao processar trabalhos com base nesse modelo.|
|los       |coleção metadataEntry   |Propriedades de extensão adicionais. A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.|

## <a name="relationships"></a>Relações
| Relação      | Tipo      |Descrição|
|:------------------|:----------|:----------|
|esquemas             |[synchronizationSchema](synchronization-synchronizationschema.md)     |Esquema de sincronização padrão para os trabalhos baseados nesse modelo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
  "suppressions": []
}
-->
