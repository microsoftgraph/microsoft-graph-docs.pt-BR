---
title: Tipo de recurso deviceManagementIntentUserStateSummary
description: Entidade que representa o resumo do estado do usuário para uma intenção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae189dbf5d5287e3123696c66cc433c41be174cc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790378"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a>Tipo de recurso deviceManagementIntentUserStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa o resumo do estado do usuário para uma intenção

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagementIntentUserStateSummary](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Leia propriedades e relações do [objeto deviceManagementIntentUserStateSummary.](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|
|[Atualizar deviceManagementIntentUserStateSummary](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|Atualize as propriedades de [um objeto deviceManagementIntentUserStateSummary.](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID|
|conflictCount|Int32|Número de usuários em conflito|
|errorCount|Int32|Número de usuários de erros|
|failedCount|Int32|Número de usuários com falha|
|notApplicableCount|Int32|Número de usuários não aplicáveis|
|successCount|Int32|Número de usuários bem-sucedidos|

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



