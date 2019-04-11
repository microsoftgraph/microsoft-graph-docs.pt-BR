---
title: tipo de recurso appLogCollectionDownloadDetails
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c581b6ffe1653c2962c03c8e6fe5d27d706882d5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784737"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a>tipo de recurso appLogCollectionDownloadDetails

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|downloadUrl|Cadeia de caracteres|Baixar a URL SAS para AppLogUploadRequest concluída|
|decryptionKey|Cadeia de caracteres|DecryptionKey como cadeia de caracteres|
|appLogDecryptionAlgorithm|[appLogDecryptionAlgorithm](../resources/intune-devices-applogdecryptionalgorithm.md)|DecryptionAlgorithm para conteúdo. Os valores possíveis são `aes256`:.|

## <a name="relationships"></a>Relações
Nenhuma

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





