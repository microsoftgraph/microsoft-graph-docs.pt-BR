---
title: tipo de recurso raProfileDatabaseEntity
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4a90d03258e4e84706d4828aaae2d10a1c064942
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124205"
---
# <a name="raprofiledatabaseentity-resource-type"></a>tipo de recurso raProfileDatabaseEntity

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar raProfileDatabaseEntities](../api/intune-rapolicy-raprofiledatabaseentity-list.md)|coleção [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)|Listar Propriedades e relações dos objetos [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) .|
|[Obter raProfileDatabaseEntity](../api/intune-rapolicy-raprofiledatabaseentity-get.md)|[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)|Leia as propriedades e as relações do objeto [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) .|
|[Criar raProfileDatabaseEntity](../api/intune-rapolicy-raprofiledatabaseentity-create.md)|[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)|Criar um novo objeto [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) .|
|[Excluir raProfileDatabaseEntity](../api/intune-rapolicy-raprofiledatabaseentity-delete.md)|Nenhum|Exclui [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md).|
|[Atualizar raProfileDatabaseEntity](../api/intune-rapolicy-raprofiledatabaseentity-update.md)|[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)|Atualiza as propriedades de um objeto [raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|versão|Int32|Ainda não documentado|
|isDeleted|Booliano|Ainda não documentado|
|softDeletedTime|DateTimeOffset|Ainda não documentado|
|displayName|Cadeia de caracteres|Ainda não documentado|
|linkedProfileIds|Coleção de GUIDs|Ainda não documentado|
|outfiletypename|String|Ainda não documentado|
|profileBody|String|Ainda não documentado|
|profileBodyHash|String|Ainda não documentado|
|platformType|Int32|Ainda não documentado|
|transformedProfileBody|String|Ainda não documentado|
|transformedProfileBodyHash|String|Ainda não documentado|
|tenantId|Guid|Ainda não documentado|
|ProfileId|Guid|Ainda não documentado|
|eTag|String|Ainda não documentado|
|schemaVersion|[raPolicyServiceVersions](../resources/intune-rapolicy-rapolicyserviceversions.md)|Ainda não documentado. Os valores possíveis são: `initial`, `betaStart`, `experimentStart`, `mmpcStart`, `iosStart`.|
|lastModified|DateTimeOffset|Ainda não documentado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.raProfileDatabaseEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
  "version": 1024,
  "isDeleted": true,
  "softDeletedTime": "String (timestamp)",
  "displayName": "String",
  "linkedProfileIds": [
    "Guid"
  ],
  "profileTypeName": "String",
  "profileBody": "String",
  "profileBodyHash": "String",
  "platformType": 1024,
  "transformedProfileBody": "String",
  "transformedProfileBodyHash": "String",
  "tenantId": "Guid",
  "profileId": "Guid",
  "eTag": "String",
  "schemaVersion": "String",
  "lastModified": "String (timestamp)"
}
```



