---
title: Tipo de recurso androidDeviceOwnerUserFacingMessage
description: Representa uma mensagem voltada para o usuário com informações de localidade, bem como uma mensagem padrão a ser usada se a localidade do usuário não corresponder a nenhuma das mensagens localizadas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07e57975a7aadf6e0d0dfe0b7479b66ef0c01d47
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213063"
---
# <a name="androiddeviceowneruserfacingmessage-resource-type"></a>Tipo de recurso androidDeviceOwnerUserFacingMessage

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa uma mensagem voltada para o usuário com informações de localidade, bem como uma mensagem padrão a ser usada se a localidade do usuário não corresponder a nenhuma das mensagens localizadas

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|localizedMessages|Coleção [keyValuePair](../resources/intune-deviceconfig-keyvaluepair.md)|A lista de <local,> de mensagens. Esta coleção pode conter um máximo de 500 elementos.|
|defaultMessage|Cadeia de Caracteres|A mensagem padrão exibida se a localidade do usuário não corresponder a nenhuma das mensagens localizadas|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerUserFacingMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerUserFacingMessage",
  "localizedMessages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "defaultMessage": "String"
}
```




