---
title: tipo de recurso microsoftStoreForBusinessAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5576f1a7aa068e0b33906944c0d9e8239a2c0f80
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732468"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a>tipo de recurso microsoftStoreForBusinessAppAssignmentSettings

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir um aplicativo móvel da Microsoft Store para Empresas a um grupo.


Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|useDeviceContext|Booliano|Se é para usar ou não o contexto de execução do dispositivo em aplicativo móvel da Microsoft Store para Empresas.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```





