---
title: Tipo de recurso cloudPcForensicStorageAccount
description: Representa uma conta de armazenamento de PC na nuvem para análise forense.
author: xhan2077
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ec722361b1d6fd1944ef22d32e2dbe38a5442741
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366299"
---
# <a name="cloudpcforensicstorageaccount-resource-type"></a>Tipo de recurso cloudPcForensicStorageAccount

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações da conta de armazenamento que podem ser usadas para armazenar um instantâneo ou instantâneos de um PC na nuvem para análise forense.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|storageAccountId|String|A ID da conta de armazenamento.|
|storageAccountName|Cadeia de caracteres|O nome da conta de armazenamento.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "storageAccountId",
  "@odata.type": "microsoft.graph.cloudPcForensicStorageAccount",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcForensicStorageAccount",
  "storageAccountId": "String",
  "storageAccountName": "String"
}
```
