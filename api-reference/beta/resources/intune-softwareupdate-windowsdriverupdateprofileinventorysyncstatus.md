---
title: Tipo de recurso windowsDriverUpdateProfileInventorySyncStatus
description: Um tipo complexo para armazenar o status de uma sincronização de inventário de perfil de driver e firmware. O status inclui a última data de sincronização bem-sucedida e o estado da última sincronização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 86bc48fd07619d7d5e99ef61239e6a92478cbd0f
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630971"
---
# <a name="windowsdriverupdateprofileinventorysyncstatus-resource-type"></a>Tipo de recurso windowsDriverUpdateProfileInventorySyncStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um tipo complexo para armazenar o status de uma sincronização de inventário de perfil de driver e firmware. O status inclui a última data de sincronização bem-sucedida e o estado da última sincronização.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastSuccessfulSyncDateTime|DateTimeOffset|A última data e hora de sincronização bem-sucedidas em UTC.|
|driverInventorySyncState|[windowsDriverUpdateProfileInventorySyncState](../resources/intune-softwareupdate-windowsdriverupdateprofileinventorysyncstate.md)|O estado da sincronização mais recente. Os valores possíveis são: `pending`, `success`, `failure`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "driverInventorySyncState": "String"
}
```




