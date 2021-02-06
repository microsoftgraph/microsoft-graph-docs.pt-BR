---
title: Tipo de recurso synchronizationTemplate
description: Fornece configurações de sincronização pré-configuradas para um aplicativo específico.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c08f5c3eee6225a1149ff993415f83b2e5916583
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132297"
---
# <a name="synchronizationtemplate-resource-type"></a>Tipo de recurso synchronizationTemplate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece configurações de sincronização pré-configuradas para um determinado aplicativo. Essas configurações serão usadas por padrão para qualquer trabalho [de](synchronization-synchronizationjob.md) sincronização baseado no modelo. O desenvolvedor do aplicativo especifica o modelo; qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o esquema [de sincronização.](synchronization-synchronizationschema.md)

Você pode fornecer vários modelos para um aplicativo e designar um modelo padrão. Se vários modelos estão disponíveis para o aplicativo em que você está interessado, procure orientações específicas do aplicativo para determinar qual deles atende melhor às suas necessidades.

## <a name="methods"></a>Métodos

| Método        | Tipo de retorno               | Descrição                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |[Coleção synchronizationTemplate](synchronization-synchronizationtemplate.md)  |Liste os modelos que estão disponíveis para uma instância de aplicativo ou aplicativo (entidade de serviço).|
|[Get](../api/synchronization-synchronizationtemplate-get.md)      |[synchronizationtemplate](synchronization-synchronizationtemplate.md)   |Leia as propriedades e os relacionamentos do **objeto synchronizationTemplate.**|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                      | Descrição                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |String                     |Identificador exclusivo do modelo.|
|ApplicationId  |Cadeia de caracteres                     |Identificador do aplicativo ao que este modelo pertence.|
|Padrão.        |Boolean                    |`true` se esse modelo for recomendado para ser o padrão para o aplicativo.|
|description    |String                     |Descrição do modelo.|
|discoverable   |String                     |`true` se esse modelo deve aparecer na coleção de modelos disponíveis para a instância do aplicativo (entidade de serviço).|
|factoryTag     |String                     |Uma das marcas de fábrica conhecidas com suporte no mecanismo de sincronização. A **factoryTag** informa ao mecanismo de sincronização qual implementação usar ao processar trabalhos baseados nesse modelo.|
|metadados       |Coleção metadataEntry   |Propriedades de extensão adicionais. A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.|

## <a name="relationships"></a>Relações
| Relação      | Tipo      |Descrição|
|:------------------|:----------|:----------|
|schema             |[synchronizationSchema](synchronization-synchronizationschema.md)     |Esquema de sincronização padrão para os trabalhos baseados neste modelo.|

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


