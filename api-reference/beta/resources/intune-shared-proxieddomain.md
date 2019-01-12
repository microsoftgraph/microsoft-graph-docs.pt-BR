---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bf4668a58e09b21c2689e10c27e773128f886b34
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971547"
---
# <a name="proxieddomain-resource-type"></a>Tipo de recurso proxiedDomain

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Domínio com proxy

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ipAddressOrFQDN|Cadeia de caracteres|O endereço IP ou o nome de domínio totalmente qualificado (FQDN).|
|proxy|Cadeia de caracteres|Endereço do proxy IP ou FQDN.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



