---
title: Tipo de recurso deviceAndAppManagementAssignedRoleDetails
description: O conjunto de Definições de Função e Atribuições de Função atribuídas a um usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9369faebceaabd27da230e4888914fee9c5e6133
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342416"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a>Tipo de recurso deviceAndAppManagementAssignedRoleDetails

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O conjunto de Definições de Função e Atribuições de Função atribuídas a um usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleDefinitionIds|Coleção String|IDs de definição de função para as Definições de Função specifc atribuídas a um usuário. Essa propriedade é somente leitura.|
|roleAssignmentIds|Coleção String|IDs de atribuição de função para as atribuições de função specifc atribuídas a um usuário. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
  "roleDefinitionIds": [
    "String"
  ],
  "roleAssignmentIds": [
    "String"
  ]
}
```




