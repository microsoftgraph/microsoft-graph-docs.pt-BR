---
title: Tipo de recurso deviceComplianceScriptRunSummary
description: Contém propriedades para o resumo de executar um script de gerenciamento de dispositivo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84bd44e53266976564f2eb4bb5ea6277cba0208c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033557"
---
# <a name="devicecompliancescriptrunsummary-resource-type"></a>Tipo de recurso deviceComplianceScriptRunSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o resumo de executar um script de gerenciamento de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceComplianceScriptRunSummary](../api/intune-devices-devicecompliancescriptrunsummary-get.md)|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Ler propriedades e relações do [objeto deviceComplianceScriptRunSummary.](../resources/intune-devices-devicecompliancescriptrunsummary.md)|
|[Atualizar deviceComplianceScriptRunSummary](../api/intune-devices-devicecompliancescriptrunsummary-update.md)|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Atualize as propriedades de [um objeto deviceComplianceScriptRunSummary.](../resources/intune-devices-devicecompliancescriptrunsummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de resumo do script de conformidade do dispositivo. Essa propriedade é somente leitura.|
|noIssueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está bem. Valores válidos -2147483648 para 2147483647|
|issueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção encontrou um problema. Valores válidos -2147483648 para 2147483647|
|detectionScriptErrorDeviceCount|Int32|Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída. Valores válidos -2147483648 para 2147483647|
|detectionScriptPendingDeviceCount|Int32|Número de dispositivos que ainda não executaram a versão mais recente do script de conformidade do dispositivo. Valores válidos -2147483648 para 2147483647|
|lastScriptRunDateTime|DateTimeOffset|Tempo de última duração do script em todos os dispositivos|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)"
}
```



