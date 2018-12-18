---
title: tipo de enum appLockerApplicationControlType
description: Valores possíveis de tipos de controle do aplicativo de AppLocker
author: tfitzmac
ms.openlocfilehash: d53c2d0f7996edfab610e4206f4d2815ba4000b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310259"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>tipo de enum appLockerApplicationControlType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis de tipos de controle do aplicativo de AppLocker
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Valor de padrão de dispositivo, nenhum tipo de controle do aplicativo selecionado.|
|enforceComponentsAndStoreApps|1|Impor o componente e armazenamento de aplicativos do Windows.|
|auditComponentsAndStoreApps|2|Auditoria do componente e armazenamento de aplicativos do Windows.|
|enforceComponentsStoreAppsAndSmartlocker|3|Aplicar os componentes do Windows, armazenar Bloqueador inteligente e aplicativos.|
|auditComponentsStoreAppsAndSmartlocker|4|Componentes do Windows de auditoria, armazenar Bloqueador inteligente e aplicativos.|



