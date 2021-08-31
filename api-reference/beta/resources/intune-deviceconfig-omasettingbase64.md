---
title: Tipo de recurso omaSettingBase64
description: Definição de Base64 das configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1fe723e83901fc982a5fe272e4a7e6422ff1cf3c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801820"
---
# <a name="omasettingbase64-resource-type"></a>Tipo de recurso omaSettingBase64

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição de Base64 das configurações de OMA.


Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|descrição|Cadeia de caracteres|Descrição. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|omaUri|Cadeia de caracteres|OMA. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|secretReferenceValueId|Cadeia de caracteres|ReferenceId para procurar segredo para descriptografia. Essa propriedade é somente leitura. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|isEncrypted|Boolean|Indica se o campo valor é criptografado. Essa propriedade é somente leitura. Herda de [omaSetting](../resources/intune-deviceconfig-omasetting.md)|
|fileName|Cadeia de caracteres|Nome de arquivo associado com a propriedade do valor (*.cer | *.crt | *.p7b | *.bin).|
|value|Cadeia de caracteres|Valor. (Cadeia de caracteres codificada em Base64)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "fileName": "String",
  "value": "String"
}
```



