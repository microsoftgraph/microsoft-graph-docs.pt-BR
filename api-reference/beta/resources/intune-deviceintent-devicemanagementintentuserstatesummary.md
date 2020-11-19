---
title: tipo de recurso deviceManagementIntentUserStateSummary
description: Entidade que representa o resumo de estado do usuário para uma intenção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fea6f40af4223bc14f7f1e419107c8b44b95f10e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275633"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a>tipo de recurso deviceManagementIntentUserStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa o resumo de estado do usuário para uma intenção

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagementIntentUserStateSummary](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Leia as propriedades e as relações do objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .|
|[Atualizar deviceManagementIntentUserStateSummary](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Atualiza as propriedades de um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID|
|conflictCount|Int32|Número de usuários em conflito|
|errorCount|Int32|Número de usuários de erro|
|failedCount|Int32|Número de usuários com falha|
|notApplicableCount|Int32|Número de usuários não aplicáveis|
|successCount|Int32|Número de usuários com êxito|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024
}
```




