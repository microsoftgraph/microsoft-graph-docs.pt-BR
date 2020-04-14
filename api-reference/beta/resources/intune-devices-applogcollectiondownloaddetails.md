---
title: tipo de recurso appLogCollectionDownloadDetails
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dade0c3a266e8cba801a8e88dacebda6bbd2d197
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465253"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a>tipo de recurso appLogCollectionDownloadDetails

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|downloadUrl|String|Baixar a URL SAS para AppLogUploadRequest concluída|
|decryptionKey|String|DecryptionKey como cadeia de caracteres|
|appLogDecryptionAlgorithm|[appLogDecryptionAlgorithm](../resources/intune-devices-applogdecryptionalgorithm.md)|DecryptionAlgorithm para conteúdo. Os valores possíveis são `aes256`:.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionDownloadDetails",
  "downloadUrl": "String",
  "decryptionKey": "String",
  "appLogDecryptionAlgorithm": "String"
}
```



