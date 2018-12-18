---
title: tipo de recurso de embeddedSIMActivationCodePool
description: Um pool representa um grupo de códigos de ativação SIM incorporados.
author: tfitzmac
ms.openlocfilehash: 9f756488d4e00e3d69bebf0e484f01aeec5650a7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307137"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a>tipo de recurso de embeddedSIMActivationCodePool

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Um pool representa um grupo de códigos de ativação SIM incorporados.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista embeddedSIMActivationCodePools](../api/intune-esim-embeddedsimactivationcodepool-list.md)|coleção [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Lista as propriedades e os relacionamentos dos objetos [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Obter embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Leia as propriedades e os relacionamentos do objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Criar embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-create.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Crie um novo objeto de [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Excluir embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-delete.md)|Nenhum|Exclui um [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).|
|[Atualizar embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-update.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Atualize as propriedades de um objeto [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Ação assign](../api/intune-esim-embeddedsimactivationcodepool-assign.md)|coleção [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para o pool de código de ativação SIM incorporado. Valor atribuído quando criado gerado pelo sistema.|
|displayName|String|O administrador definida pelo nome do pool de código de ativação SIM incorporado.|
|createdDateTime|DateTimeOffset|A hora em que o pool de código de ativação SIM incorporado foi criado. Lado de serviço gerado.|
|modifiedDateTime|DateTimeOffset|A hora em que o pool de código de ativação SIM incorporado foi modificado pela última vez. Lado de serviços atualizado.|
|activationCodes|coleção [embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)|Os códigos de ativação que pertencem a esse pool. Esta propriedade de navegação é usada para postar códigos de ativação para Intune, mas não pode ser usada para ler códigos de ativação do Intune.|
|activationCodeCount|Int32|A contagem total dos códigos de ativação que pertencem a esse pool.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Propriedade navegação para uma lista de destinos ao qual esse pool é atribuído.|
|deviceStates|coleção [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Propriedade navegação para uma lista de estados de dispositivo para este pool.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePool"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "String",
      "matchingIdentifier": "String",
      "smdpPlusServerAddress": "String"
    }
  ],
  "activationCodeCount": 1024
}
```





