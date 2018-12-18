---
title: tipo de enum actionState
description: Estado da ação no dispositivo
author: tfitzmac
ms.openlocfilehash: 1f36c3a6709ade5860ff24cc8d10c2cb0294a471
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315103"
---
# <a name="actionstate-enum-type"></a>tipo de enum actionState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Estado da ação no dispositivo
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Não é um estado de ação válido|
|pendente|1|A ação é pendente|
|cancelado|2|Ação foi cancelada.|
|ativo|3|Ação está ativa.|
|done|4|Ação concluída sem erros.|
|Falha|5|Falha na ação|
|notSupported|6|Não há suporte para a ação.|





