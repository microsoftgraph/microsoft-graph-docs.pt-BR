---
title: tipo de recurso groupPolicyMigrationReport
description: O relatório de migração de política de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 038c0f81999bebbf0d2406637bb71e03a67397ce
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539201"
---
# <a name="grouppolicymigrationreport-resource-type"></a>tipo de recurso groupPolicyMigrationReport

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O relatório de migração de política de grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyMigrationReports](../api/intune-gpanalyticsservice-grouppolicymigrationreport-list.md)|coleção [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Listar Propriedades e relações dos objetos [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .|
|[Obter groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-get.md)|[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Leia as propriedades e as relações do objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .|
|[Criar groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-create.md)|[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Criar um novo objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .|
|[Excluir groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-delete.md)|Nenhum|Exclui [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).|
|[Atualizar groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-update.md)|[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Atualiza as propriedades de um objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .|
|[ação createMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-createmigrationreport.md)|String|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|
|groupPolicyObjectId|Guid|O GUID do objeto da política de grupo do conteúdo XML do GPO|
|displayName|String|O nome do objeto de diretiva de grupo do conteúdo XML do GPO|
|ouDistinguishedName|Cadeia de caracteres|O nome diferenciado da OU.|
|createdDateTime|DateTimeOffset|A data e a hora em que o GroupPolicyMigrationReport foi criado.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o GroupPolicyMigrationReport foi modificado pela última vez.|
|groupPolicyCreatedDateTime|DateTimeOffset|A data e a hora em que o GroupPolicyMigrationReport foi criado.|
|groupPolicyLastModifiedDateTime|DateTimeOffset|A data e a hora em que o GroupPolicyMigrationReport foi modificado pela última vez.|
|migrationReadiness|[groupPolicyMigrationReadiness](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|A cobertura do Intune para o arquivo de objeto de diretiva de grupo associado. Os valores possíveis são: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|targetedInActiveDirectory|Booliano|A propriedade de destino no AD do conteúdo XML do GPO|
|totalSettingsCount|Int32|O número total de configurações de política de grupo do arquivo de GPO.|
|supportedSettingsCount|Int32|O número de configurações de política de grupo compatíveis com o Intune.|
|supportedSettingsPercent|Int32|A porcentagem de configurações de política de grupo compatíveis com o Intune.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupPolicySettingMappings|coleção [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Uma lista de configurações de política de grupo para mapeamentos MDM/Intune.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyMigrationReport"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "String (identifier)",
  "groupPolicyObjectId": "Guid",
  "displayName": "String",
  "ouDistinguishedName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "groupPolicyCreatedDateTime": "String (timestamp)",
  "groupPolicyLastModifiedDateTime": "String (timestamp)",
  "migrationReadiness": "String",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 1024,
  "supportedSettingsCount": 1024,
  "supportedSettingsPercent": 1024
}
```



