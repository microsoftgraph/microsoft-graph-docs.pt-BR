---
title: tipo de recurso de windowsKioskAzureADGroup
description: A classe usada para identificar um grupo de AzureAD para a configuração de quiosque
author: tfitzmac
ms.openlocfilehash: 3c4cdd8388c71b5f051ea8338e82123c241ec429
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339519"
---
# <a name="windowskioskazureadgroup-resource-type"></a>tipo de recurso de windowsKioskAzureADGroup

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

A classe usada para identificar um grupo de AzureAD para a configuração de quiosque

Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome para exibição do grupo AzureAD que será bloqueado para esta configuração de quiosque|
|groupId|String|A ID do grupo AzureAD que será bloqueado para esta configuração de quiosque|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```





