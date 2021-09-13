---
title: Tipo de recurso deviceManagementScript
description: O Intune fornecerá ao cliente a capacidade de executar seus scripts do Powershell nos dispositivos inscritos do Windows 10 Azure Active Directory ingressados. O script pode ser executado uma vez ou periodicamente.
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 12dfae8bfe0a4d005e0871a7ca91d91301f87624
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039060"
---
# <a name="devicemanagementscript-resource-type"></a>Tipo de recurso deviceManagementScript

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Intune fornecerá ao cliente a capacidade de executar seus scripts do Powershell nos dispositivos inscritos do Windows 10 Azure Active Directory ingressados. O script pode ser executado uma vez ou periodicamente.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementScripts](../api/intune-shared-devicemanagementscript-list.md)|[Coleção deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Listar propriedades e relações dos [objetos deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)|
|[Obter deviceManagementScript](../api/intune-shared-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Leia propriedades e relações do [objeto deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)|
|[Criar deviceManagementScript](../api/intune-shared-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Crie um novo [objeto deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)|
|[Excluir deviceManagementScript](../api/intune-shared-devicemanagementscript-delete.md)|Nenhum|Exclui um [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).|
|[Atualizar deviceManagementScript](../api/intune-shared-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Atualize as propriedades de um [objeto deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)|
|**Gerenciamento de dispositivo**|
|[atribuir ação](../api/intune-shared-devicemanagementscript-assign.md)|Nenhuma|Ainda não documentado|
|**Conjunto de Políticas**|
|[Ação hasPayloadLinks](../api/intune-shared-devicemanagementscript-haspayloadlinks.md)|[coleção hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do script de gerenciamento de dispositivos.|
|displayName|Cadeia de caracteres|Nome do script de gerenciamento de dispositivos.|
|description|Cadeia de caracteres|Descrição opcional para o script de gerenciamento de dispositivos.|
|scriptContent|Binário|O conteúdo do script.|
|createdDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivos foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o script de gerenciamento de dispositivos foi modificado pela última vez. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Boleano|Indique se a assinatura de script precisa ser verificada.|
|fileName|String|Nome do arquivo de script.|
|roleScopeTagIds|String collection|Lista de IDs de marca de escopo para esta instância do PowerShellScript.|
|runAs32Bit|Boleano|Um valor que indica se o script do PowerShell deve ser executado como 32 bits|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Gerenciamento de dispositivo**|
|groupAssignments|[Coleção deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivos.|
|assignments|[Coleção deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|A lista de atribuições de grupo para o script de gerenciamento de dispositivos.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Execute o resumo do script de gerenciamento de dispositivos.|
|deviceRunStates|[Coleção deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Lista de estados de executar para esse script em todos os dispositivos.|
|userRunStates|[Coleção deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Lista de estados de executar para esse script em todos os usuários.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "runAs32Bit": true
}
```



