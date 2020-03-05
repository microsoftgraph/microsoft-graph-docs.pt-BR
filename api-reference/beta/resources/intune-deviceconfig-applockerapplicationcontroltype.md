---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 07ce6969c79581ed33b3a34d75445f7bf5612598
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527076"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>tipo de enumeração appLockerApplicationControlType

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis dos tipos de controle do aplicativo AppLocker

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.|
|enforceComponentsAndStoreApps|1 |Aplicar o componente do Windows e armazenar aplicativos.|
|auditComponentsAndStoreApps|2 |Auditar o componente do Windows e armazenar aplicativos.|
|enforceComponentsStoreAppsAndSmartlocker|3 |Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.|
|auditComponentsStoreAppsAndSmartlocker|4 |Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.|



