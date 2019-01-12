---
title: tipo de enum defenderThreatAction
description: Ação de padrão do Defender assuma detectadas ameaças de Malware.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: fb54523f2817da328854e57a6672045e46ceb266
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938080"
---
# <a name="defenderthreataction-enum-type"></a>tipo de enum defenderThreatAction

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ação de padrão do Defender assuma detectadas ameaças de Malware.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Aplica a ação com base na definição de atualização.|
|clean|1|Limpe ameaça detectada.|
|quarentena|2|Quarentena ameaça detectada.|
|remover|3|Remova ameaça detectada.|
|permitir|4|Permitir ameaça detectada.|
|userDefined|5|Permitir que o usuário determinar a ação a ser executada com ameaça detectada.|
|bloquear|6|Bloquear ameaça detectada.|





