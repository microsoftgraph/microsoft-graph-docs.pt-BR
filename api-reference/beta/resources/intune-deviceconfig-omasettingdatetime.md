---
title: Tipo de recurso omaSettingDateTime
description: Definição de datetime para configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1efe2ae812842d0c0bd3c0e3d7c28c1931a3ff95
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790896"
---
# <a name="omasettingdatetime-resource-type"></a>Tipo de recurso omaSettingDateTime

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de datetime para configurações de OMA.


Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|descrição|Cadeia de caracteres|Descrição. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|Cadeia de caracteres|OMA. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|secretReferenceValueId|Cadeia de caracteres|ReferenceId para procurar segredo para descriptografia. Essa propriedade é somente leitura. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|isEncrypted|Boolean|Indica se o campo valor é criptografado. Essa propriedade é somente leitura. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|value|DateTimeOffset|Valor.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": "String (timestamp)"
}
```



