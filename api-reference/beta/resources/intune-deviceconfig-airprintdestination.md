---
title: tipo de recurso de airPrintDestination
description: Representa um destino AirPrint.
author: tfitzmac
ms.openlocfilehash: 046f85c65d382b34e6920f30f6b2718f817371a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361051"
---
# <a name="airprintdestination-resource-type"></a>tipo de recurso de airPrintDestination

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa um destino AirPrint.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ipAddress|Cadeia de caracteres|O endereço IP de destino AirPrint.|
|resourcePath|String|O caminho do recurso associado à impressora. Isso corresponde ao parâmetro rp do registro Bonjour _ipps.tcp. Por exemplo: impressoras/Canon_MG5300_series, impressoras/Xerox_Phaser_7600, ipp/impressão, Epson_IPP_Printer.|
|porta|Int32|A porta de escuta do destino AirPrint. Se essa chave não for especificado, AirPrint usará a porta padrão. Disponível no iOS 11.0 e versões posteriores.|
|forceTls|Boolean|Se true conexões de AirPrint são protegidas pela segurança de camada de transporte (TLS). O padrão é false. Disponível no iOS 11.0 e versões posteriores.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.airPrintDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.airPrintDestination",
  "ipAddress": "String",
  "resourcePath": "String",
  "port": 1024,
  "forceTls": true
}
```





