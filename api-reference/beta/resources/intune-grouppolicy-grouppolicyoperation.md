---
title: Tipo de recurso groupPolicyOperation
description: A entidade representa uma operação de política de grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b469baabe89ea5a05477fb1734fe0bfc4b2a63d103cb050efb541cac020e6f0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251166"
---
# <a name="grouppolicyoperation-resource-type"></a>Tipo de recurso groupPolicyOperation

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa uma operação de política de grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyOperations](../api/intune-grouppolicy-grouppolicyoperation-list.md)|[coleção groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Listar propriedades e relações dos [objetos groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)|
|[Obter groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-get.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Ler propriedades e relações do [objeto groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)|
|[Criar groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-create.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Crie um novo [objeto groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)|
|[Excluir groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-delete.md)|Nenhum|Exclui um [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md).|
|[Atualizar groupPolicyOperation](../api/intune-grouppolicy-grouppolicyoperation-update.md)|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Atualize as propriedades de [um objeto groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|operationType|[groupPolicyOperationType](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|O tipo de operação de política de grupo. Os valores possíveis são: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.|
|operationStatus|[groupPolicyOperationStatus](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|O status da operação de política de grupo. Os valores possíveis são: `unknown`, `inProgress`, `success`, `failed`.|
|statusDetails|Cadeia de caracteres|O detalhe do status da operação de política de grupo.|
|id|Cadeia de caracteres|Chave da entidade.|
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




