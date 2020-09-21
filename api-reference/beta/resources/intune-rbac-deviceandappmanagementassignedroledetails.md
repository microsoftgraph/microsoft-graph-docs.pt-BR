---
title: tipo de recurso deviceAndAppManagementAssignedRoleDetails
description: O conjunto de definições de função e atribuições de função atribuídas a um usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f9dff637f950d980b3fc0de89ecfde26da6b40de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070797"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a>tipo de recurso deviceAndAppManagementAssignedRoleDetails

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O conjunto de definições de função e atribuições de função atribuídas a um usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleDefinitionIds|Coleção de cadeias de caracteres|IDs de definição de função para as definições de função especialmente atribuídas a um usuário.|
|roleAssignmentIds|Coleção de cadeias de caracteres|IDs de atribuição de função para as atribuições de função especialmente atribuídas a um usuário.|

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






