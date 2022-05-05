---
title: Tipo de recurso androidFotaDeploymentAssignment
description: Descreve o grupo de segurança de implantação ao qual atribuir uma implantação. O back-end expandirá a ID do Grupo de Segurança para extrair números de série do dispositivo antes de enviar uma solicitação de criação de implantação para Zebra.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c159840ba5bb2035223a45f0dec54a94055a2176
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213047"
---
# <a name="androidfotadeploymentassignment-resource-type"></a>Tipo de recurso androidFotaDeploymentAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve o grupo de segurança de implantação ao qual atribuir uma implantação. O back-end expandirá a ID do Grupo de Segurança para extrair números de série do dispositivo antes de enviar uma solicitação de criação de implantação para Zebra.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres| Chave para a entidade de atribuição de FOTA do Android|
|destino|[androidFotaDeploymentAssignmentTarget](../resources/intune-androidfotaservice-androidfotadeploymentassignmenttarget.md)|O AAD grupo no qual estamos implantando atualizações de firmware|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidFotaDeploymentAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidFotaDeploymentAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.androidFotaDeploymentAssignmentTarget",
    "groupId": "String"
  }
}
```




