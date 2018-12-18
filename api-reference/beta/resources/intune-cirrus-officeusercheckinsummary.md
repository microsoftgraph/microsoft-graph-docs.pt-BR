---
title: tipo de recurso de officeUserCheckinSummary
description: Entidade que descreve as estatísticas de check-in do inquilino.
author: tfitzmac
ms.openlocfilehash: 5064882f74a13feca726a6ebb91c34cf9a85af86
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306325"
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



