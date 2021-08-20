---
title: Tipo de recurso macOSSoftwareUpdateStateSummary
description: Resumo do estado de atualização de software macOS para um dispositivo e usuário
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 17355d6b166ce85e781015d3ad63c963ca09b198a755fdc0723f86086d1e9ef1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236364"
---
# <a name="macossoftwareupdatestatesummary-resource-type"></a>Tipo de recurso macOSSoftwareUpdateStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo do estado de atualização de software macOS para um dispositivo e usuário

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSSoftwareUpdateStateSummaries](../api/intune-deviceconfig-macossoftwareupdatestatesummary-list.md)|[Coleção macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Listar propriedades e relações dos [objetos macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|
|[Obter macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-get.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Leia propriedades e relações do [objeto macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|
|[Criar macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-create.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Crie um novo [objeto macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|
|[Excluir macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-delete.md)|Nenhum|Exclui um [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).|
|[Atualizar macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-update.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Atualize as propriedades de [um objeto macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|displayName|Cadeia de caracteres|Nome acessível humano da atualização de software|
|productKey|String|Chave do produto da atualização de software.|
|updateCategory|[macOSSoftwareUpdateCategory](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|Categoria de atualização de software. Os valores possíveis são: `critical`, `configurationDataFile`, `firmware`, `other`.|
|updateVersion|Cadeia de caracteres|Versão da atualização de software|
|state|[macOSSoftwareUpdateState](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|Estado da atualização de software. Os valores possíveis são: `success` , , , , , , , , , `downloading` , , `downloaded` , , , `installing` `idle` `available` , `scheduled` `downloadFailed` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installInsufficientSpace` `installInsufficientPower` `installFailed` `commandFailed` .|
|lastUpdatedDateTime|DateTimeOffset|Última data em que o relatório para este dispositivo e a chave do produto foi atualizado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "productKey": "String",
  "updateCategory": "String",
  "updateVersion": "String",
  "state": "String",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




