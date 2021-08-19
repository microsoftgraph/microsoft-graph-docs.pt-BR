---
title: tipo de recurso numberRange
description: Definição de Intervalo de Números.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 39cd34613a87f4ebfca5d1a432a80fde1027843ceb55d51b8dad329ea6b7d251
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54133352"
---
# <a name="numberrange-resource-type"></a>tipo de recurso numberRange

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de Intervalo de Números.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lowerNumber|Int32|Número inferior.|
|upperNumber|Int32|Número superior.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```




