---
title: tipo de enum appLockerApplicationControlType
description: Valores possíveis de tipos de controle do aplicativo de AppLocker
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cb1fbb6ffe2ffc1841ebb4aa5ac1df91b762a788
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933572"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>tipo de enum appLockerApplicationControlType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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





