---
title: Tipo de recurso deviceComplianceScript
description: O Intune fornecerá ao cliente a capacidade de executar seus scripts de Conformidade (detecção) do Powershell nos dispositivos inscritos do Windows 10 Azure Active Directory ingressados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88b82fe497653e5c2ee0f2d796773b00dbe66cc5163fe5ebdf62a422322e23e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126925"
---
# <a name="devicecompliancescript-resource-type"></a>Tipo de recurso deviceComplianceScript

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Intune fornecerá ao cliente a capacidade de executar seus scripts de Conformidade (detecção) do Powershell nos dispositivos inscritos do Windows 10 Azure Active Directory ingressados.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceComplianceScripts](../api/intune-devices-devicecompliancescript-list.md)|[Coleção deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Listar propriedades e relações dos objetos [deviceComplianceScript.](../resources/intune-devices-devicecompliancescript.md)|
|[Obter deviceComplianceScript](../api/intune-devices-devicecompliancescript-get.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Leia propriedades e relações do [objeto deviceComplianceScript.](../resources/intune-devices-devicecompliancescript.md)|
|[Criar deviceComplianceScript](../api/intune-devices-devicecompliancescript-create.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Crie um novo [objeto deviceComplianceScript.](../resources/intune-devices-devicecompliancescript.md)|
|[Excluir deviceComplianceScript](../api/intune-devices-devicecompliancescript-delete.md)|Nenhum|Exclui um [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md).|
|[Atualizar deviceComplianceScript](../api/intune-devices-devicecompliancescript-update.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Atualize as propriedades de um [objeto deviceComplianceScript.](../resources/intune-devices-devicecompliancescript.md)|
|[atribuir ação](../api/intune-devices-devicecompliancescript-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do script de conformidade do dispositivo|
|publicador|String|Nome do editor de scripts de conformidade do dispositivo|
|versão|String|Versão do script de conformidade do dispositivo|
|displayName|Cadeia de caracteres|Nome do script de conformidade do dispositivo|
|description|Cadeia de caracteres|Descrição do script de conformidade do dispositivo|
|detectionScriptContent|Binário|Todo o conteúdo do script do powershell de detecção|
|createdDateTime|DateTimeOffset|O data/hora de quando o script de conformidade do dispositivo foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|O data/hora de quando o script de conformidade do dispositivo foi modificado. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Boolean|Indicar se a assinatura de script precisa ser verificada|
|runAs32Bit|Boolean|Indicar se os scripts do PowerShell devem ser executados como 32 bits|
|roleScopeTagIds|String collection|Lista de IDs de marca de escopo para o script de conformidade do dispositivo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|A lista de atribuições de grupo para o script de conformidade do dispositivo|
|runSummary|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Resumo de executar de alto nível para o script de conformidade do dispositivo.|
|deviceRunStates|[Coleção deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Lista de estados de executar para o script de conformidade do dispositivo em todos os dispositivos|

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




