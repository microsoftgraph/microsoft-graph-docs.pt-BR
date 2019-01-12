---
title: tipo de enum windowsUserAccountControlSettings
description: Valores possíveis para configurações de controle de conta de usuário do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd16db4236096687ddcc9f169dd657c938fd6815
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911809"
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





