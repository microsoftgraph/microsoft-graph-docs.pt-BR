---
title: Tipo de recurso embeddedSIMActivationCodePool
description: Um pool representa um grupo de códigos de ativação de SIM incorporados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9358f29c20db8614c396850913c21711ffa16e90520999573cef46faac874630
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244677"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a>Tipo de recurso embeddedSIMActivationCodePool

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um pool representa um grupo de códigos de ativação de SIM incorporados.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar embeddedSIMActivationCodePools](../api/intune-esim-embeddedsimactivationcodepool-list.md)|[Coleção embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Listar propriedades e relações dos [objetos embeddedSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)|
|[Obter embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Leia propriedades e relações do [objeto embeddedSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)|
|[Criar embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-create.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Crie um novo [objeto embeddedSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)|
|[Excluir embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-delete.md)|Nenhum|Exclui um [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).|
|[Atualizar embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-update.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Atualize as propriedades de [um objeto EMBEDDEDSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) incorporado.|
|[atribuir ação](../api/intune-esim-embeddedsimactivationcodepool-assign.md)|[Coleção embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para o pool de código de ativação do SIM incorporado. Valor gerado pelo sistema atribuído quando criado.|
|displayName|Cadeia de caracteres|O nome definido pelo administrador do pool de código de ativação do SIM incorporado.|
|createdDateTime|DateTimeOffset|A hora em que o pool de código de ativação do SIM incorporado foi criado. Lado de serviço gerado.|
|modifiedDateTime|DateTimeOffset|A hora em que o pool de código de ativação do SIM incorporado foi modificado pela última vez. Lado do serviço atualizado.|
|activationCodes|[Coleção embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)|Os códigos de ativação que pertencem a esse pool. Essa propriedade de navegação é usada para postar códigos de ativação no Intune, mas não pode ser usada para ler códigos de ativação do Intune.|
|activationCodeCount|Int32|A contagem total de códigos de ativação que pertencem a esse pool.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Propriedade de navegação para uma lista de destinos aos quais esse pool é atribuído.|
|deviceStates|[Coleção embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Propriedade de navegação para uma lista de estados de dispositivo para este pool.|

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




