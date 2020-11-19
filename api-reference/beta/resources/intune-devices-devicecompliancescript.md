---
title: tipo de recurso deviceComplianceScript
description: O Intune fornecerá ao cliente a capacidade de executar os scripts de conformidade do PowerShell (detecção) nos dispositivos associados do Windows 10 Azure Active Directory inscrito.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f1eab8a7483c2c029f00edd6c481d0028da3ad9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267688"
---
# <a name="devicecompliancescript-resource-type"></a>tipo de recurso deviceComplianceScript

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Intune fornecerá ao cliente a capacidade de executar os scripts de conformidade do PowerShell (detecção) nos dispositivos associados do Windows 10 Azure Active Directory inscrito.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceComplianceScripts](../api/intune-devices-devicecompliancescript-list.md)|coleção [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Listar Propriedades e relações dos objetos [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) .|
|[Obter deviceComplianceScript](../api/intune-devices-devicecompliancescript-get.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Leia as propriedades e as relações do objeto [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) .|
|[Criar deviceComplianceScript](../api/intune-devices-devicecompliancescript-create.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Criar um novo objeto [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) .|
|[Excluir deviceComplianceScript](../api/intune-devices-devicecompliancescript-delete.md)|Nenhum|Exclui [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md).|
|[Atualizar deviceComplianceScript](../api/intune-devices-devicecompliancescript-update.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Atualiza as propriedades de um objeto [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) .|
|[atribuir ação](../api/intune-devices-devicecompliancescript-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do script de conformidade do dispositivo|
|publicador|String|Nome do editor de scripts de conformidade de dispositivos|
|versão|String|Versão do script de conformidade do dispositivo|
|displayName|String|Nome do script de conformidade do dispositivo|
|description|String|Descrição do script de conformidade do dispositivo|
|detectionScriptContent|Binária|Todo o conteúdo do script do PowerShell de detecção|
|createdDateTime|DateTimeOffset|O carimbo de data/hora de quando o script de conformidade do dispositivo foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|O carimbo de data/hora de quando o script de conformidade do dispositivo foi modificado. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Booliano|Indicar se a assinatura do script precisa ser verificada|
|runAs32Bit|Booliano|Indicar se os scripts do PowerShell devem ser executados como 32 bits|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para o script de conformidade do dispositivo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|A lista de atribuições de grupo para o script de conformidade do dispositivo|
|runSummary|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Resumo de execução de alto nível para o script de conformidade do dispositivo.|
|deviceRunStates|coleção [deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Lista de Estados de execução para o script de conformidade de dispositivo em todos os dispositivos|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "id": "String (identifier)",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




