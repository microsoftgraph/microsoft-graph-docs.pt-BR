---
title: Tipo de recurso deviceHealthScriptRunSummary
description: Contém propriedades para o resumo de executar um script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b1c1b31413c19436c7dceb34a2055a238fe5881a
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665228"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a>Tipo de recurso deviceHealthScriptRunSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o resumo de executar um script de gerenciamento de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Leia propriedades e relações do [objeto deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)|
|[Atualizar deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Atualize as propriedades de [um objeto deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade resumo do script de saúde do dispositivo. Essa propriedade é somente leitura.|
|noIssueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está saudável|
|issueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção encontrou um problema|
|detectionScriptErrorDeviceCount|Int32|Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída|
|detectionScriptPendingDeviceCount|Int32|Número de dispositivos que ainda não executaram a versão mais recente do script de saúde do dispositivo|
|detectionScriptNotApplicableDeviceCount|Int32|Número de dispositivos para os quais o script de detecção não foi aplicável|
|issueRemediatedDeviceCount|Int32|Número de dispositivos para os quais o script de correção foi capaz de resolver o problema detectado|
|remediationSkippedDeviceCount|Int32|Número de dispositivos para os quais a correção foi ignorada|
|issueReoccurredDeviceCount|Int32|Número de dispositivos para os quais o script de correção foi executado com êxito, mas não conseguiu resolver o problema detectado|
|remediationScriptErrorDeviceCount|Int32|Número de dispositivos para os quais a execução do script de correção encontrou um erro e não foi concluída|
|lastScriptRunDateTime|DateTimeOffset|Tempo de última duração do script em todos os dispositivos|
|issueRemediatedCumulativeDeviceCount|Int32|Número de dispositivos que foram remediados nos últimos 30 dias|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "detectionScriptNotApplicableDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```




