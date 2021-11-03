---
title: Tipo de recurso androidManagedStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da Loja Gerenciada do Android a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a2afa3243cc19b016430e2b9960f6aecc349cdf
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60691537"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a>Tipo de recurso androidManagedStoreAppAssignmentSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades usadas para atribuir um aplicativo móvel da Loja Gerenciada do Android a um grupo.


Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|androidManagedStoreAppTrackIds|Coleção de cadeias de caracteres|As IDs de faixa para habilitar para essa atribuição de aplicativo.|
|autoUpdateMode|[androidManagedStoreAutoUpdateMode](../resources/intune-shared-androidmanagedstoreautoupdatemode.md)|A priorização de atualizações automáticas para essa atribuição de aplicativo. Os valores possíveis são: `default`, `postponed`, `priority`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppAssignmentSettings",
  "androidManagedStoreAppTrackIds": [
    "String"
  ],
  "autoUpdateMode": "String"
}
```



