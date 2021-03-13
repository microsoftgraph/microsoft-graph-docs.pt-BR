---
title: Tipo de recurso connectionInfo
description: O objeto connectionInfo define as informações de conexão usadas para se comunicar com um recurso.
author: hanki-microsoft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8bbab1e93cf5af0fcfbd401b6b726f3165f595b4
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761813"
---
# <a name="connectioninfo-resource-type"></a>Tipo de recurso connectionInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
