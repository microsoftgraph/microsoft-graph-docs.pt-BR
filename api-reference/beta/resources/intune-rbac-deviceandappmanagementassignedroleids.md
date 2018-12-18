---
title: tipo de recurso de deviceAndAppManagementAssignedRoleIds
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 034120b891812a43c6c1683f61e52f071dc89816
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353379"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a>tipo de recurso de deviceAndAppManagementAssignedRoleIds

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleDefinitionIds|Coleção de GUIDs|IDs de definição de função para o specifc definições de função atribuída a um usuário.|
|roleAssignmentIds|Coleção de GUIDs|IDs de atribuição de função para o specifc atribuições de função atribuída a um usuário.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleIds",
  "roleDefinitionIds": [
    "Guid"
  ],
  "roleAssignmentIds": [
    "Guid"
  ]
}
```





