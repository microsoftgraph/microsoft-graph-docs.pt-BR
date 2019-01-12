---
title: tipo de enum actionState
description: Estado da ação no dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5579d8de986a764cd96e42dff30c007449130b0b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922442"
---
# <a name="actionstate-enum-type"></a>tipo de enum actionState

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Estado da ação no dispositivo
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhum|0|Não é um estado de ação válido|
|pendente|1|A ação é pendente|
|cancelado|2|Ação foi cancelada.|
|ativo|3|Ação está ativa.|
|done|4|Ação concluída sem erros.|
|Falha|5|Falha na ação|
|notSupported|6|Não há suporte para a ação.|



