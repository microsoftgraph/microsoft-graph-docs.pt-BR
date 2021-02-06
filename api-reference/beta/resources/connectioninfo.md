---
title: Tipo de recurso connectionInfo
description: O objeto connectionInfo define as informações de conexão usadas para se comunicar com um recurso.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 454dc7fcd045bb91819b39ad30f603191bab8380
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137699"
---
# <a name="connectioninfo-resource-type"></a>Tipo de recurso connectionInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O objeto connectionInfo define o localizador de recursos usado para se comunicar com um recurso no Gerenciamento de Direitos do Azure AD.

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
