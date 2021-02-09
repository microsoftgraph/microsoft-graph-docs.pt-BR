---
title: Tipo de recurso assignmentFilterEvaluationStatusDetails
description: Uma classe que contém informações sobre as cargas em que o filtro foi aplicado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b569b59ad929c0928edecb90c7ef05432fbc082
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160163"
---
# <a name="assignmentfilterevaluationstatusdetails-resource-type"></a>Tipo de recurso assignmentFilterEvaluationStatusDetails

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém informações sobre as cargas em que o filtro foi aplicado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar assignmentFilterEvaluationStatusDetailses](../api/intune-policyset-assignmentfilterevaluationstatusdetails-list.md)|[Coleção assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|Listar propriedades e relações dos objetos [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|
|[Obter assignmentFilterEvaluationStatusDetails](../api/intune-policyset-assignmentfilterevaluationstatusdetails-get.md)|[assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|Ler propriedades e relações do objeto [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|
|[Criar assignmentFilterEvaluationStatusDetails](../api/intune-policyset-assignmentfilterevaluationstatusdetails-create.md)|[assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|Criar um novo [objeto assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|
|[Excluir assignmentFilterEvaluationStatusDetails](../api/intune-policyset-assignmentfilterevaluationstatusdetails-delete.md)|Nenhum(a)|Exclui [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md).|
|[Atualizar assignmentFilterEvaluationStatusDetails](../api/intune-policyset-assignmentfilterevaluationstatusdetails-update.md)|[assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|Atualizar as propriedades de um [objeto assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade AssignmentFilterEvaluationStatusDetails.|
|payloadId|String|PayloadId no qual o filtro foi aplicado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.assignmentFilterEvaluationStatusDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "id": "String (identifier)",
  "payloadId": "String"
}
```




