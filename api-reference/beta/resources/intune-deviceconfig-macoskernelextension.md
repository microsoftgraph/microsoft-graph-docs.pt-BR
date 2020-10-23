---
title: tipo de recurso macOSKernelExtension
description: Representa uma extensão de kernel macOS específica. Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22d37a87a8cdc33791907d305eca36d8ceb0fb8c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701470"
---
# <a name="macoskernelextension-resource-type"></a>tipo de recurso macOSKernelExtension

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa uma extensão de kernel macOS específica. Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|teamIdentifier|String|O identificador de equipe que foi usado para assinar a extensão do kernel.|
|bundleId|String|ID do pacote da extensão do kernel.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKernelExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKernelExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```





