---
title: Tipo de recurso macOSKernelExtension
description: Representa uma extensão de kernel do macOS específica. Uma extensão de kernel macOS pode ser descrita pelo identificador de equipe, além do identificador de pacote.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb01902173135d20ac1568006c398de88ea8b1061f35681f70c51b5b7dc23ceb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244992"
---
# <a name="macoskernelextension-resource-type"></a>Tipo de recurso macOSKernelExtension

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa uma extensão de kernel do macOS específica. Uma extensão de kernel macOS pode ser descrita pelo identificador de equipe, além do identificador de pacote.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|teamIdentifier|Cadeia de caracteres|O identificador de equipe usado para assinar a extensão do kernel.|
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




