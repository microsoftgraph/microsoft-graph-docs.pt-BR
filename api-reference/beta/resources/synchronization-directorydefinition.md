---
title: Tipo de recurso directoryDefinition
description: Fornece informações do mecanismo de sincronização sobre um diretório e seus objetos.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 8e3adb4679233fa35a53574b6f8d0c2b806be110
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956796"
---
# <a name="directorydefinition-resource-type"></a>Tipo de recurso directoryDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece informações do mecanismo de sincronização sobre um diretório e seus objetos. Esse recurso informa ao mecanismo de sincronização, por exemplo, que o diretório tem objetos denominados **usuário** e grupo **,** quais atributos são suportados para esses objetos e os tipos para esses atributos. Para que o objeto e [](synchronization-synchronizationrule.md) o atributo participem de regras de sincronização e mapeamentos de objetos, eles devem ser [definidos](synchronization-objectmapping.md)como parte da definição de diretório.

Em geral, o [esquema](synchronization-synchronizationschema.md) de sincronização [](synchronization-synchronizationtemplate.md) padrão fornecido como parte do modelo de sincronização definirá os objetos e atributos mais usados para esse diretório. No entanto, se o diretório suportar a adição de atributos personalizados, talvez você queira expandir a definição padrão com seus próprios objetos ou atributos personalizados. Para obter mais informações, consulte [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and Configure [synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).

As definições de diretório são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Descobrir directoryDefinition](../api/directorydefinition-discover.md) | [directoryDefinition](synchronization-directorydefinition.md) |Descubra o esquema e as propriedades suportadas do diretório.|

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|id           |Cadeia de caracteres     |Identificador de diretório. Não anulável.|
|metadados       |Coleção metadataEntry    |Propriedades de extensão adicionais. A menos que mencionado explicitamente, os valores de metadados não devem ser alterados.|
|nome           |Cadeia de caracteres     |Nome do diretório. Deve ser exclusivo no esquema [de sincronização](synchronization-synchronizationschema.md). Não anulável.|
|objects        |[coleção objectDefinition](synchronization-objectdefinition.md)    |Coleção de objetos suportados pelo diretório.|
|versão|String|Valor somente leitura que indica a versão descoberta. `null` se a descoberta ainda não tiver ocorrido.|
|discoveryDateTime|DateTimeOffset| Representa a data e a hora de descoberta usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|discoverabilities|directoryDefinitionDiscoverabilities| Valor somente leitura indicando que tipo de descoberta o aplicativo oferece suporte. Os possíveis valores são: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.| 

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


