---
title: Tipo de recurso vpnServer
description: Definição do Servidor VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b620b47742d8f5bc64eeacee361683cf0676950ff85839941c9972e8a4c91277
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139625"
---
# <a name="vpnserver-resource-type"></a>Tipo de recurso vpnServer

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definição do Servidor VPN.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|Descrição.|
|address|Cadeia de caracteres|Endereço (endereço IP, FQDN ou URL)|
|isDefaultServer|Boolean|Servidor padrão.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```




