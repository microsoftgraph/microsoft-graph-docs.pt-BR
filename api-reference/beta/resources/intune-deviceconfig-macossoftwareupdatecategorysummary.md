---
title: Tipo de recurso macOSSoftwareUpdateCategorySummary
description: Relatório de resumo de categoria de atualização de software macOS para um dispositivo e usuário
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f8d084eccf6e253c258f7ddd14c1c09feaa1ad2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095560"
---
# <a name="macossoftwareupdatecategorysummary-resource-type"></a>Tipo de recurso macOSSoftwareUpdateCategorySummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Relatório de resumo de categoria de atualização de software macOS para um dispositivo e usuário

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSSoftwareUpdateCategorySummaries](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-list.md)|[Coleção macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Listar propriedades e relações dos [objetos macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|
|[Obter macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-get.md)|[macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Leia propriedades e relações do [objeto macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|
|[Criar macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-create.md)|[macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Crie um novo [objeto macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|
|[Excluir macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-delete.md)|Nenhum|Exclui um [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md).|
|[Atualizar macOSSoftwareUpdateCategorySummary](../api/intune-deviceconfig-macossoftwareupdatecategorysummary-update.md)|[macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Atualize as propriedades de [um objeto macOSSoftwareUpdateCategorySummary.](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|displayName|Cadeia de caracteres|O nome do relatório|
|deviceId|Cadeia de caracteres|A ID do dispositivo.|
|userId|Cadeia de caracteres|A ID do usuário.|
|updateCategory|[macOSSoftwareUpdateCategory](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|Tipo de atualização de software. Os valores possíveis são: `critical`, `configurationDataFile`, `firmware`, `other`.|
|successfulUpdateCount|Int32|Número de atualizações bem-sucedidas no dispositivo|
|failedUpdateCount|Int32|Número de atualizações com falha no dispositivo|
|totalUpdateCount|Int32|Número de atualizações totais no dispositivo|
|lastUpdatedDateTime|DateTimeOffset|Última data em que o relatório deste dispositivo foi atualizado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|updateStateSummaries|[Coleção macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Resumo dos estados de atualização.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateCategorySummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "id": "String (identifier)",
  "displayName": "String",
  "deviceId": "String",
  "userId": "String",
  "updateCategory": "String",
  "successfulUpdateCount": 1024,
  "failedUpdateCount": 1024,
  "totalUpdateCount": 1024,
  "lastUpdatedDateTime": "String (timestamp)"
}
```



