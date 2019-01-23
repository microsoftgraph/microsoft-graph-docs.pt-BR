---
title: tipo de recurso de officeUserCheckinSummary
description: Entidade que descreve as estatísticas de check-in do inquilino.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d44c978ff1442c98038bf627397de5ca3a0ca3bf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411005"
---
# <a name="officeusercheckinsummary-resource-type"></a>tipo de recurso de officeUserCheckinSummary

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Entidade que descreve as estatísticas de check-in do inquilino.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|succeededUserCount|Int32|Total de usuários bem-sucedida verificar ins nos últimos 3 meses.|
|failedUserCount|Int32|Total de usuários com falha verificar ins nos últimos 3 meses.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



