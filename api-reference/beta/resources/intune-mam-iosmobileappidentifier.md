---
title: Tipo de recurso iosMobileAppIdentifier
description: O identificador de um aplicativo iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fabff3ec78d64f87eb68b961557bff3752d1339d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49297816"
---
# <a name="iosmobileappidentifier-resource-type"></a>Tipo de recurso iosMobileAppIdentifier

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O identificador de um aplicativo iOS.


Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|bundleId|Cadeia de caracteres|O identificador de um aplicativo, conforme especificado na App Store.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```




