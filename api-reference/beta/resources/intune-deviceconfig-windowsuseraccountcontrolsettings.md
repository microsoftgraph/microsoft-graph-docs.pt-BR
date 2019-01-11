---
title: tipo de enum windowsUserAccountControlSettings
description: Valores possíveis para configurações de controle de conta de usuário do Windows.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2803e2d15b907fc2a05303be8a0b4e4db4ce66f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861450"
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





