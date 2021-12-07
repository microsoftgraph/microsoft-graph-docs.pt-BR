---
title: Tipo de recurso microsoftManagedDesktop
description: Representa configurações específicas para a Área de Trabalho Gerenciada da Microsoft que permite aos clientes obter uma experiência de dispositivo gerenciado para um computador na nuvem.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 26eadd11fc46ba794249f1d6f1094a000777b5cf
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322744"
---
# <a name="microsoftmanageddesktop-resource-type"></a>Tipo de recurso microsoftManagedDesktop

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa configurações específicas para a Área de Trabalho Gerenciada da Microsoft que permite aos clientes obter uma experiência de dispositivo gerenciado para um computador na nuvem.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|perfil|String|O nome do perfil da Área de Trabalho Gerenciada da Microsoft ao Windows 365 Cloud PC está associado.|
|type|[microsoftManagedDesktopType](#microsoftmanageddesktoptype-values)|Indica se a política de provisionamento habilita a Área de Trabalho Gerenciada da Microsoft. Indica o tipo de plano no qual o dispositivo é gerenciado se a política de provisionamento estiver habilitada. Os valores possíveis são: `notManaged`, `premiumManaged`, `standardManaged`, `starterManaged`, `unknownFutureValue`.|

### <a name="microsoftmanageddesktoptype-values"></a>valores microsoftManagedDesktopType

|Member|Descrição|
|:---|:---|
|notManaged|O dispositivo não é gerenciado pela Área de Trabalho Gerenciada da Microsoft.|
|premiumManaged|O dispositivo é gerenciado pelo plano premium da Área de Trabalho Gerenciada da Microsoft.|
|standardManaged|O dispositivo é gerenciado pelo plano padrão da Área de Trabalho Gerenciada da Microsoft.|
|starterManaged|O dispositivo é gerenciado pelo plano inicial da Área de Trabalho Gerenciada da Microsoft.|
|unknownFutureValue|Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftManagedDesktop"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.microsoftManagedDesktop",
  "type": "String",
  "profile": "String"
}
```
