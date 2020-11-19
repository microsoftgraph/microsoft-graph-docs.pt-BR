---
title: tipo de recurso macOSSoftwareUpdateStateSummary
description: Resumo do estado de atualização do software MacOS para um dispositivo e usuário
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb7cebab56f9866753794259b70a0bdd8cc1e414
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279812"
---
# <a name="macossoftwareupdatestatesummary-resource-type"></a>tipo de recurso macOSSoftwareUpdateStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Resumo do estado de atualização do software MacOS para um dispositivo e usuário

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSSoftwareUpdateStateSummaries](../api/intune-deviceconfig-macossoftwareupdatestatesummary-list.md)|coleção [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Listar Propriedades e relações dos objetos [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .|
|[Obter macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-get.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Leia as propriedades e as relações do objeto [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .|
|[Criar macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-create.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Criar um novo objeto [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .|
|[Excluir macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-delete.md)|Nenhum|Exclui [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).|
|[Atualizar macOSSoftwareUpdateStateSummary](../api/intune-deviceconfig-macossoftwareupdatestatesummary-update.md)|[macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)|Atualiza as propriedades de um objeto [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|displayName|String|Nome da atualização de software legível por pessoas|
|productKey|String|Chave de produto da atualização de software.|
|updateCategory|[macOSSoftwareUpdateCategory](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|Categoria de atualização de software. Os valores possíveis são: `critical`, `configurationDataFile`, `firmware`, `other`.|
|updateVersion|String|Versão da atualização de software|
|state|[macOSSoftwareUpdateState](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|Estado da atualização de software. Os valores possíveis são:, `success` `downloading` , `downloaded` , `installing` , `idle` , `available` , `scheduled` , `downloadFailed` , `downloadInsufficientSpace` , `downloadInsufficientPower` , `downloadInsufficientNetwork` , `installInsufficientSpace` ,, `installInsufficientPower` `installFailed` `commandFailed` .|
|lastUpdatedDateTime|DateTimeOffset|Hora da última data em que o relatório para este dispositivo e chave do produto foi atualizado.|

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




