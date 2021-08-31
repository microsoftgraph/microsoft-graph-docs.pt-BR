---
title: Tipo de recurso deviceHealthScript
description: O Intune fornecerá ao cliente a capacidade de executar seus scripts de Saúde do Powershell (correção + detecção) nos dispositivos inscritos do Windows 10 Azure Active Directory ingressados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0a8dd615f783be39f02949d9535bcefdda5d2b64
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58799455"
---
# <a name="devicehealthscript-resource-type"></a>Tipo de recurso deviceHealthScript

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Intune fornecerá ao cliente a capacidade de executar seus scripts de Saúde do Powershell (correção + detecção) nos dispositivos inscritos do Windows 10 Azure Active Directory ingressados.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceHealthScripts](../api/intune-devices-devicehealthscript-list.md)|[Coleção deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Listar propriedades e relações dos [objetos deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)|
|[Obter deviceHealthScript](../api/intune-devices-devicehealthscript-get.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Leia propriedades e relações do [objeto deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)|
|[Criar deviceHealthScript](../api/intune-devices-devicehealthscript-create.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Crie um novo [objeto deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)|
|[Excluir deviceHealthScript](../api/intune-devices-devicehealthscript-delete.md)|Nenhum(a)|Exclui um [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).|
|[Atualizar deviceHealthScript](../api/intune-devices-devicehealthscript-update.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Atualize as propriedades de um [objeto deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)|
|[atribuir ação](../api/intune-devices-devicehealthscript-assign.md)|Nenhuma|Ainda não documentado|
|[Ação updateGlobalScript](../api/intune-devices-devicehealthscript-updateglobalscript.md)|Cadeia de caracteres|Atualizar o Script de Saúde do Dispositivo Proprietário|
|[ação getGlobalScriptHighestAvailableVersion](../api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion.md)|Cadeia de caracteres|Atualizar o Script de Saúde do Dispositivo Proprietário|
|[Ação enableGlobalScripts](../api/intune-devices-devicehealthscript-enableglobalscripts.md)|Nenhuma|Ainda não documentado|
|[função areGlobalScriptsAvailable](../api/intune-devices-devicehealthscript-areglobalscriptsavailable.md)|[globalDeviceHealthScriptState](../resources/intune-devices-globaldevicehealthscriptstate.md)|Ainda não documentado|
|[função getRemediationSummary](../api/intune-devices-devicehealthscript-getremediationsummary.md)|[deviceHealthScriptRemediationSummary](../resources/intune-devices-devicehealthscriptremediationsummary.md)|Ainda não documentado|
|[função getRemediationHistory](../api/intune-devices-devicehealthscript-getremediationhistory.md)|[deviceHealthScriptRemediationHistory](../resources/intune-devices-devicehealthscriptremediationhistory.md)|Função para obter o número de correções por scripts de saúde de um dispositivo|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do script de saúde do dispositivo|
|publicador|String|Nome do editor de scripts de saúde do dispositivo|
|versão|String|Versão do script de saúde do dispositivo|
|displayName|Cadeia de caracteres|Nome do script de saúde do dispositivo|
|descrição|Cadeia de caracteres|Descrição do script de saúde do dispositivo|
|detectionScriptContent|Binário|Todo o conteúdo do script do powershell de detecção|
|remediationScriptContent|Binário|Todo o conteúdo do script do powershell de correção|
|createdDateTime|DateTimeOffset|O timestamp de quando o script de saúde do dispositivo foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|O data/hora de quando o script de saúde do dispositivo foi modificado. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Boleano|Indicar se a assinatura de script precisa ser verificada|
|runAs32Bit|Boleano|Indicar se os scripts do PowerShell devem ser executados como 32 bits|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para o script de saúde do dispositivo|
|isGlobalScript|Boleano|Determina se esse é o Script Proprietário da Microsoft. Scripts proprietários são somente leitura|
|highestAvailableVersion|Cadeia de caracteres|Versão mais alta disponível para um script proprietário da Microsoft|
|detectionScriptParameters|[Coleção deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|Lista de objetos ComplexType DetectionScriptParameters.|
|remediationScriptParameters|[Coleção deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|Lista de objetos ComplexType RemediationScriptParameters.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|A lista de atribuições de grupo para o script de saúde do dispositivo|
|runSummary|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Resumo de executar de alto nível para script de saúde do dispositivo.|
|deviceRunStates|[Coleção deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Lista de estados de executar para o script de saúde do dispositivo em todos os dispositivos|

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



