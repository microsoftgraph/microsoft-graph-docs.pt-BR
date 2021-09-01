---
title: Tipo de recurso deviceAndAppManagementAssignedRoleDetails
description: O conjunto de Definições de Função e Atribuições de Função atribuídas a um usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88d69e52049eb1dd90eeb6657e3403369ff4a14f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806009"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a>Tipo de recurso deviceAndAppManagementAssignedRoleDetails

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O conjunto de Definições de Função e Atribuições de Função atribuídas a um usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleDefinitionIds|Coleção de cadeias de caracteres|IDs de definição de função para as Definições de Função specifc atribuídas a um usuário. Essa propriedade é somente leitura.|
|roleAssignmentIds|Coleção de cadeias de caracteres|IDs de atribuição de função para as atribuições de função specifc atribuídas a um usuário. Essa propriedade é somente leitura.|

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



