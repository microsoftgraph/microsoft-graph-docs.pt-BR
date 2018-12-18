---
title: tipo de enum windowsUserAccountControlSettings
description: Valores possíveis para configurações de controle de conta de usuário do Windows.
author: tfitzmac
ms.openlocfilehash: dcec2ca6e5b6401b5277e513867c0646bff79c21
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320297"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a>tipo de enum windowsUserAccountControlSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para configurações de controle de conta de usuário do Windows.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Definido pelo usuário, valor padrão, sem intenção.|
|alwaysNotify|1|Sempre notifica.|
|notifyOnAppChanges|2|Notifica sobre alterações de aplicativo.|
|notifyOnAppChangesWithoutDimming|3|Notifica sobre mudanças de app sem escurecer a área de trabalho.|
|neverNotify|4|Nunca notifica.|





