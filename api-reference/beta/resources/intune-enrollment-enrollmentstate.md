---
title: tipo de enum enrollmentState
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9394755c5b6e6de8ed039b226d03074f1ef16cc3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933586"
---
# <a name="enrollmentstate-enum-type"></a>tipo de enum enrollmentState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ainda não documentado
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|0|O estado de inscrição do dispositivo é desconhecido|
|inscritos|1|Inscrever-se o dispositivo.|
|pendingReset|2|Inscritos, mas ele está inscrito via perfil de inscrição e o perfil registrado é diferente do perfil atribuído.|
|Falha|3|Não inscritos e não houver registro de falha de inscrição.|
|notContacted|4|Dispositivo é importado, mas não inscritos.|
|bloqueado|5|Dispositivo está inscrito como userless, mas seja bloqueado para mover para a inscrição do usuário porque o aplicativo falha na instalação.|





