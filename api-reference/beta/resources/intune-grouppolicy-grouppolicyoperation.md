---
title: tipo de recurso groupPolicyOperation
description: A entidade representa uma operação de política de grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 186fc43e61dff934771469c621d1b77583535d4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030987"
---
# <a name="grouppolicyoperation-resource-type"></a>tipo de recurso groupPolicyOperation

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa uma operação de política de grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyOperations](../api/intune-grouppolicy-grouppolicyoperation-list.md)|coleção [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Listar Propriedades e relações dos objetos [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) .|
|[Obter groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-get.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Leia as propriedades e as relações do objeto [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) .|
|[Criar groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-create.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Criar um novo objeto [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) .|
|[Excluir groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-delete.md)|Nenhum|Exclui [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md).|
|[Atualizar groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-update.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Atualiza as propriedades de um objeto [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|OperationType|[groupPolicyOperationType](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|O tipo de operação de política de grupo. Os valores possíveis são: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.|
|operationStatus|[groupPolicyOperationStatus](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|O status da operação da política de grupo. Os valores possíveis são: `unknown`, `inProgress`, `success`, `failed`.|
|statusDetails|String|Detalhes do status da operação da política de grupo.|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "String",
  "operationStatus": "String",
  "statusDetails": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```






