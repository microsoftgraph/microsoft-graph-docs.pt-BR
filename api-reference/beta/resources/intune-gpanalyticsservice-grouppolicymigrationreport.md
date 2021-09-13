---
title: Tipo de recurso groupPolicyMigrationReport
description: O relatório de migração da Política de Grupo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb50a01e3f812b1e4e5cb6b986ef52d4ec1817de
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086243"
---
# <a name="grouppolicymigrationreport-resource-type"></a>Tipo de recurso groupPolicyMigrationReport

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O relatório de migração da Política de Grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyMigrationReports](../api/intune-gpanalyticsservice-grouppolicymigrationreport-list.md)|[coleção groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Listar propriedades e relações dos [objetos groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|
|[Obter groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-get.md)|[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Ler propriedades e relações do [objeto groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|
|[Criar groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-create.md)|[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Crie um novo [objeto groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|
|[Excluir groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-delete.md)|Nenhum|Exclui um [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).|
|[Atualizar groupPolicyMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-update.md)|[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|Atualize as propriedades de [um objeto groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)|
|[Ação createMigrationReport](../api/intune-gpanalyticsservice-grouppolicymigrationreport-createmigrationreport.md)|String|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|
|groupPolicyObjectId|Guid|O GUID do objeto de política de grupo do conteúdo XML do GPO|
|displayName|Cadeia de caracteres|O nome do Objeto de Política de Grupo do Conteúdo XML do GPO|
|ouDistinguishedName|Cadeia de Caracteres|O nome diferenciado da UO.|
|createdDateTime|DateTimeOffset|A data e a hora em que o GroupPolicyMigrationReport foi criado.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que GroupPolicyMigrationReport foi modificada pela última vez.|
|groupPolicyCreatedDateTime|DateTimeOffset|A data e a hora em que o GroupPolicyMigrationReport foi criado.|
|groupPolicyLastModifiedDateTime|DateTimeOffset|A data e a hora em que GroupPolicyMigrationReport foi modificada pela última vez.|
|migrationReadiness|[groupPolicyMigrationReadiness](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|A cobertura do Intune para o arquivo de Objeto de Política de Grupo associado. Os valores possíveis são: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|targetedInActiveDirectory|Boleano|A propriedade Targeted in AD do Conteúdo XML do GPO|
|totalSettingsCount|Int32|O número total de políticas de grupo Configurações do arquivo GPO.|
|supportedSettingsCount|Int32|O número de políticas de grupo Configurações com suporte do Intune.|
|supportedSettingsPercent|Int32|O Percentual de políticas de grupo Configurações com suporte do Intune.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupPolicySettingMappings|[coleção groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)|Uma lista de configurações de política de grupo para mapeamentos MDM/Intune.|
|unsupportedGroupPolicyExtensions|[coleção unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|Uma lista de extensões de política de grupo sem suporte dentro do Objeto de Política de Grupo.|

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



