---
title: Tipo de recurso deviceHealthScript
description: Intune fornecerá ao cliente a capacidade de executar seus scripts de Integridade do Powershell (correção + detecção) nos dispositivos ingressados no Azure Active Directory do Windows 10.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01250fa2ad479de8fbe37eed627fbda2b6ddb24c
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670811"
---
# <a name="devicehealthscript-resource-type"></a>Tipo de recurso deviceHealthScript

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Intune fornecerá ao cliente a capacidade de executar seus scripts de Integridade do Powershell (correção + detecção) nos dispositivos ingressados no Azure Active Directory do Windows 10.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceHealthScripts](../api/intune-devices-devicehealthscript-list.md)|[Coleção deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Listar propriedades e relações dos [objetos deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Obter deviceHealthScript](../api/intune-devices-devicehealthscript-get.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Ler propriedades e relações do objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Criar deviceHealthScript](../api/intune-devices-devicehealthscript-create.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Crie um novo [objeto deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Excluir deviceHealthScript](../api/intune-devices-devicehealthscript-delete.md)|Nenhum|Exclui um [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).|
|[Atualizar deviceHealthScript](../api/intune-devices-devicehealthscript-update.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Atualize as propriedades de um [objeto deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[atribuir ação](../api/intune-devices-devicehealthscript-assign.md)|Nenhuma|Ainda não documentado|
|[Ação updateGlobalScript](../api/intune-devices-devicehealthscript-updateglobalscript.md)|Cadeia de Caracteres|Atualizar o script de integridade do dispositivo proprietário|
|[Ação getGlobalScriptHighestAvailableVersion](../api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion.md)|Cadeia de Caracteres|Atualizar o script de integridade do dispositivo proprietário|
|[Ação enableGlobalScripts](../api/intune-devices-devicehealthscript-enableglobalscripts.md)|Nenhuma|Ainda não documentado|
|[Função areGlobalScriptsAvailable](../api/intune-devices-devicehealthscript-areglobalscriptsavailable.md)|[globalDeviceHealthScriptState](../resources/intune-devices-globaldevicehealthscriptstate.md)|Ainda não documentado|
|[Função getRemediationSummary](../api/intune-devices-devicehealthscript-getremediationsummary.md)|[deviceHealthScriptRemediationSummary](../resources/intune-devices-devicehealthscriptremediationsummary.md)|Ainda não documentado|
|[Função getRemediationHistory](../api/intune-devices-devicehealthscript-getremediationhistory.md)|[deviceHealthScriptRemediationHistory](../resources/intune-devices-devicehealthscriptremediationhistory.md)|Função para obter o número de correções por scripts de integridade do dispositivo|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para o script de integridade do dispositivo|
|publicador|String|Nome do editor de script de integridade do dispositivo|
|versão|String|Versão do script de integridade do dispositivo|
|displayName|String|Nome do script de integridade do dispositivo|
|descrição|Cadeia de caracteres|Descrição do script de integridade do dispositivo|
|detectionScriptContent|Binária|Todo o conteúdo do script do PowerShell de detecção|
|remediationScriptContent|Binária|Todo o conteúdo do script do PowerShell de correção|
|createdDateTime|DateTimeOffset|O carimbo de data/hora de quando o script de integridade do dispositivo foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|O carimbo de data/hora de quando o script de integridade do dispositivo foi modificado. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-devices-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Booleano|Indicar se a assinatura de script precisa ser verificada|
|runAs32Bit|Booleano|Indicar se os scripts do PowerShell devem ser executados como 32 bits|
|roleScopeTagIds|String collection|Lista de IDs de marca de escopo para o script de integridade do dispositivo|
|isGlobalScript|Booleano|Determina se este é o Script Proprietário da Microsoft. Scripts proprietários são somente leitura|
|highestAvailableVersion|Cadeia de Caracteres|Versão mais alta disponível para um script proprietário da Microsoft|
|detectionScriptParameters|[Coleção deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|Lista de objetos DetectionScriptParameters ComplexType.|
|remediationScriptParameters|[Coleção deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|Lista de objetos ComplexType RemediationScriptParameters.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|A lista de atribuições de grupo para o script de integridade do dispositivo|
|runSummary|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Resumo de execução de alto nível para o script de integridade do dispositivo.|
|deviceRunStates|[coleção deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Lista de estados de execução para o script de integridade do dispositivo em todos os dispositivos|

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
  "highestAvailableVersion": "String",
  "detectionScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "String",
      "description": "String",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "String"
    }
  ],
  "remediationScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "String",
      "description": "String",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "String"
    }
  ]
}
```




