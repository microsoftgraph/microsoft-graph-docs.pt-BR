---
title: tipo de recurso de officeUserCheckinSummary
description: Entidade que descreve as estatísticas de check-in do inquilino.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 374f5113a517b52ae7af6381f575ac60e5d00ae4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946578"
---
# <a name="officeusercheckinsummary-resource-type"></a>tipo de recurso de officeUserCheckinSummary

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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



