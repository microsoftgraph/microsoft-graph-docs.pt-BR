---
title: tipo de enum appLockerApplicationControlType
description: Valores possíveis de tipos de controle do aplicativo de AppLocker
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3bc89620a6dd13a65cfe40f37ba2f775e6a9c83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425719"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>tipo de enum appLockerApplicationControlType

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Valores possíveis de tipos de controle do aplicativo de AppLocker

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|não-configuradas|0|Valor de padrão de dispositivo, nenhum tipo de controle do aplicativo selecionado.|
|enforceComponentsAndStoreApps|1|Impor o componente e armazenamento de aplicativos do Windows.|
|auditComponentsAndStoreApps|2|Auditoria do componente e armazenamento de aplicativos do Windows.|
|enforceComponentsStoreAppsAndSmartlocker|3|Aplicar os componentes do Windows, armazenar Bloqueador inteligente e aplicativos.|
|auditComponentsStoreAppsAndSmartlocker|4|Componentes do Windows de auditoria, armazenar Bloqueador inteligente e aplicativos.|




