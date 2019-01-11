---
title: Tipo de recurso managedAppConfiguration
description: Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b3acf921f76e34e21427364ef84d1647cc7d0f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861317"
---
# <a name="managedappconfiguration-resource-type"></a>Tipo de recurso managedAppConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração usada para distribuir um conjunto de configurações personalizadas, no estado em que se encontram, para os usuários aos quais a configuração está com escopo definido

Herda de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppConfigurations](../api/intune-mam-managedappconfiguration-list.md)|Coleção [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)|Lista propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).|
|[Obter managedAppConfiguration](../api/intune-mam-managedappconfiguration-get.md)|[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)|Propriedades de leitura e relações do objeto [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome para exibição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|Cadeia de caracteres|A descrição da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|Última vez em que a política foi modificada. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|Cadeia de caracteres|Versão da entidade. Herdado de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|customSettings|Coleção [keyValuePair](../resources/intune-mam-keyvaluepair.md)|Um conjunto de pares de chave de cadeia de caracteres e valor de cadeia de caracteres a serem enviados aos aplicativos para usuários para os quais a configuração tem escopo definido, não alterados por esse serviço|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



