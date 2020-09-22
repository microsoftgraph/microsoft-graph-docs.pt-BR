---
title: tipo de recurso directoryDefinition
description: Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ccafa9d6763339c32102ace1572c85148f793fc6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089284"
---
# <a name="directorydefinition-resource-type"></a>tipo de recurso directoryDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece as informações do mecanismo de sincronização sobre um diretório e seus objetos. Esse recurso instrui o mecanismo de sincronização, por exemplo, que o diretório tem objetos chamados **usuário** e **grupo**, quais atributos são compatíveis com esses objetos e os tipos desses atributos. Para que o objeto e o atributo participem das [regras de sincronização](synchronization-synchronizationrule.md) e dos [mapeamentos de objetos](synchronization-objectmapping.md), eles devem ser definidos como parte da definição de diretório.

Em geral, o [esquema de sincronização](synchronization-synchronizationschema.md) padrão fornecido como parte do [modelo de sincronização](synchronization-synchronizationtemplate.md) definirá os objetos e atributos usados com mais frequência para esse diretório. No entanto, se o diretório oferecer suporte à adição de atributos personalizados, convém expandir a definição padrão com seus próprios objetos ou atributos personalizados. Para obter mais informações, consulte [Configurar a sincronização com atributos personalizados](synchronization-configure-with-custom-target-attributes.md) e [Configurar a sincronização com atributos de extensão de diretório](synchronization-configure-with-directory-extension-attributes.md).

As definições de diretório são atualizadas como parte do [esquema de sincronização](synchronization-synchronizationschema.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Descobrir directoryDefinition](../api/directorydefinition-discover.md) | [directoryDefinition](synchronization-directorydefinition.md) |Descubra o esquema e as propriedades com suporte do diretório.|

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|id           |Cadeia de caracteres     |Identificador de diretório. Não anulável.|
|los       |coleção metadataEntry    |Propriedades de extensão adicionais. A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.|
|name           |Cadeia de caracteres     |Nome do diretório. Deve ser exclusivo no [esquema de sincronização](synchronization-synchronizationschema.md). Não anulável.|
|objectos        |coleção [ObjectDefinition](synchronization-objectdefinition.md)    |Conjunto de objetos suportados pelo diretório.|
|versão|String|Valor somente leitura que indica a versão descoberta. NULL se a descoberta ainda não tiver ocorrido.|
|discoveryDateTime|DateTimeOffset| Representa a data e a hora da descoberta usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|discoverabilities|cadeia de caracteres| Valor somente leitura indicando qual tipo de descoberta o aplicativo oferece suporte. Os possíveis valores são: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.| 

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


