---
title: Tipo de recurso directoryDefinition
description: Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 77af192ff09cf557eec3e73c1973c4c71dc39a96
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134047"
---
# <a name="directorydefinition-resource-type"></a>Tipo de recurso directoryDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos. Esse recurso informa ao mecanismo de sincronização, por  exemplo, que o diretório tem objetos chamados usuário e **grupo,** quais atributos são suportados para esses objetos e os tipos para esses atributos. Para que o objeto e [](synchronization-synchronizationrule.md) o atributo participem de regras de sincronização e mapeamentos de objetos, eles devem ser [definidos](synchronization-objectmapping.md)como parte da definição de diretório.

Em geral, o [esquema](synchronization-synchronizationschema.md) de sincronização [](synchronization-synchronizationtemplate.md) padrão fornecido como parte do modelo de sincronização definirá os objetos e atributos mais usados para esse diretório. No entanto, se o diretório suportar a adição de atributos personalizados, talvez você queira expandir a definição padrão com seus próprios objetos ou atributos personalizados. Para obter mais informações, [consulte Configurar a sincronização com atributos personalizados](synchronization-configure-with-custom-target-attributes.md) e [configurar a sincronização com atributos de extensão de diretório.](synchronization-configure-with-directory-extension-attributes.md)

As definições de diretório são atualizadas como parte [do esquema de sincronização.](synchronization-synchronizationschema.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Descobrir directoryDefinition](../api/directorydefinition-discover.md) | [directoryDefinition](synchronization-directorydefinition.md) |Descubra o esquema e as propriedades com suporte do diretório.|

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|id           |String     |Identificador de diretório. Não anulável.|
|metadados       |Coleção metadataEntry    |Propriedades de extensão adicionais. A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.|
|nome           |String     |Nome do diretório. Deve ser exclusivo no esquema [de sincronização.](synchronization-synchronizationschema.md) Não anulável.|
|objects        |[coleção objectDefinition](synchronization-objectdefinition.md)    |Coleção de objetos com suporte no diretório.|
|versão|String|Valor somente leitura que indica a versão descoberta. Nulo se a descoberta ainda não tiver ocorrido.|
|discoveryDateTime|DateTimeOffset| Representa a data e a hora de descoberta usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|discoverabilities|string| Valor somente leitura indicando que tipo de descoberta o aplicativo oferece suporte. Os possíveis valores são: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.| 

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "discoverabilities": "String",
  "discoveryDateTime": "DateTimeOffset",
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}],
  "version": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


