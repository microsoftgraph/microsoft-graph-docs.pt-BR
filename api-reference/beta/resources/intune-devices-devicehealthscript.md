---
title: tipo de recurso deviceHealthScript
description: O Intune fornecerá ao cliente a capacidade de executar os scripts de integridade do PowerShell (remediation + detecção) nos dispositivos do Windows 10 Azure Active Directory associados registrados.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0ed7d3adf5386e4e56782b1aafd71f3bd08a6b92
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538473"
---
# <a name="devicehealthscript-resource-type"></a>tipo de recurso deviceHealthScript

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Intune fornecerá ao cliente a capacidade de executar os scripts de integridade do PowerShell (remediation + detecção) nos dispositivos do Windows 10 Azure Active Directory associados registrados.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceHealthScripts](../api/intune-devices-devicehealthscript-list.md)|coleção [deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Listar Propriedades e relações dos objetos [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Obter deviceHealthScript](../api/intune-devices-devicehealthscript-get.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Leia as propriedades e as relações do objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Criar deviceHealthScript](../api/intune-devices-devicehealthscript-create.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Criar um novo objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Excluir deviceHealthScript](../api/intune-devices-devicehealthscript-delete.md)|Nenhum|Exclui [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).|
|[Atualizar deviceHealthScript](../api/intune-devices-devicehealthscript-update.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Atualiza as propriedades de um objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[atribuir ação](../api/intune-devices-devicehealthscript-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do script de integridade do dispositivo|
|publicador|Cadeia de caracteres|Nome do editor de script de integridade do dispositivo|
|versão|String|Versão do script de integridade do dispositivo|
|displayName|Cadeia de caracteres|Nome do script de integridade do dispositivo|
|description|String|Descrição do script de integridade do dispositivo|
|detectionScriptContent|Binária|Todo o conteúdo do script do PowerShell de detecção|
|remediationScriptContent|Binária|Todo o conteúdo do script do PowerShell de correção|
|createdDateTime|DateTimeOffset|O carimbo de data/hora de quando o script de integridade do dispositivo foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|O carimbo de data/hora de quando o script de integridade do dispositivo foi modificado. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Booliano|Indicar se a assinatura do script precisa ser verificada|
|runAs32Bit|Booliano|Indicar se os scripts do PowerShell devem ser executados como 32 bits|
|roleScopeTagIds|String collection|Lista de IDs de marcas de escopo para o script de integridade do dispositivo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|A lista de atribuições de grupo para o script de integridade do dispositivo|
|runSummary|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Resumo de execução de alto nível para o script de integridade do dispositivo.|
|deviceRunStates|coleção [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Lista de Estados de execução para o script de integridade do dispositivo em todos os dispositivos|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "String (identifier)",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
  "remediationScriptContent": "binary",
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



