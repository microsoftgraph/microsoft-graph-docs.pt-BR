---
title: tipo de recurso de synchronizationTemplate
description: " qualquer pessoa pode recuperar o modelo para ver as configurações padrão, incluindo o esquema de sincronização."
ms.openlocfilehash: 90850ad43fdd14fc38ff6ae8cfa97f47806a289d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037230"
---
# <a name="synchronizationtemplate-resource-type"></a>tipo de recurso de synchronizationTemplate

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
|metadados       |coleção metadataEntry   |Propriedades adicionais de extensão. A menos que mencionado explicitamente, valores de metadados não devem ser alterados.|

## <a name="relationships"></a>Relações
| Relação      | Tipo      |Descrição|
|:------------------|:----------|:----------|
|esquema             |[synchronizationSchema](synchronization-synchronizationschema.md)     |Esquema de sincronização padrão para os trabalhos baseados nesse modelo.|

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->