---
title: tipo de recurso deviceHealthScript
description: O Intune fornecerá ao cliente a capacidade de executar os scripts de integridade do PowerShell (remediation + detecção) nos dispositivos do Windows 10 Azure Active Directory associados registrados.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c9b375299db9fa52be494dca185ba9370627e3cb
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159476"
---
# <a name="devicehealthscript-resource-type"></a>tipo de recurso deviceHealthScript

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|[ação updateGlobalScript](../api/intune-devices-devicehealthscript-updateglobalscript.md)|String|Atualizar o script de integridade do dispositivo proprietário|
|[ação getGlobalScriptHighestAvailableVersion](../api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion.md)|String|Atualizar o script de integridade do dispositivo proprietário|
|[ação enableGlobalScripts](../api/intune-devices-devicehealthscript-enableglobalscripts.md)|Nenhuma|Ainda não documentado|
|[função areGlobalScriptsAvailable](../api/intune-devices-devicehealthscript-areglobalscriptsavailable.md)|[globalDeviceHealthScriptState](../resources/intune-devices-globaldevicehealthscriptstate.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do script de integridade do dispositivo|
|publicador|String|Nome do editor de script de integridade do dispositivo|
|versão|String|Versão do script de integridade do dispositivo|
|displayName|Cadeia de caracteres|Nome do script de integridade do dispositivo|
|descrição|String|Descrição do script de integridade do dispositivo|
|detectionScriptContent|Binária|Todo o conteúdo do script do PowerShell de detecção|
|remediationScriptContent|Binária|Todo o conteúdo do script do PowerShell de correção|
|createdDateTime|DateTimeOffset|O carimbo de data/hora de quando o script de integridade do dispositivo foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|O carimbo de data/hora de quando o script de integridade do dispositivo foi modificado. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Booliano|Indicar se a assinatura do script precisa ser verificada|
|runAs32Bit|Booliano|Indicar se os scripts do PowerShell devem ser executados como 32 bits|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marcas de escopo para o script de integridade do dispositivo|
|isGlobalScript|Booliano|Determina se este é o script proprietário da Microsoft. Scripts proprietários são somente leitura|
|highestAvailableVersion|String|Versão mais recente disponível para um script proprietário da Microsoft|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|A lista de atribuições de grupo para o script de integridade do dispositivo|
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
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "String"
}
```



