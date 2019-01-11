---
title: tipo de recurso de extendedKeyUsage
description: Definição de uso estendido de chave personalizada
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f1fd159a9b9fdb621a1e52bd080c005c8b93129c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840975"
---
# <a name="extendedkeyusage-resource-type"></a>tipo de recurso de extendedKeyUsage

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Definição de uso estendido de chave personalizada
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|name|Cadeia de caracteres|Nome do uso estendido de chave|
|objectIdentifier|Cadeia de caracteres|Identificador de objeto de uso da chave de estendido|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```





