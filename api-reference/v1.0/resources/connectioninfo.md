---
title: Tipo de recurso connectionInfo
description: O objeto connectionInfo define as informações de conexão usadas para se comunicar com um recurso.
author: hanki-microsoft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4c00cf41bd89deebf4b1453cb4f7389094e3dcb8
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242173"
---
# <a name="connectioninfo-resource-type"></a>Tipo de recurso connectionInfo

Namespace: microsoft.graph


O objeto connectionInfo define o localizador de recursos usado para se comunicar com um recurso no Azure AD Entitlement Management.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|url|Cadeia de caracteres|O ponto de extremidade usado pelo Gerenciamento de Direitos para se comunicar com o recurso do pacote de acesso.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.connectionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectionInfo",
  "url": "String"
}
```


