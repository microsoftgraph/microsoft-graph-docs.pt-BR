---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b1e463959cf4b5b39076fcf200b1c61ea0e73c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575125"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>tipo de enumeração appLockerApplicationControlType

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis dos tipos de controle do aplicativo AppLocker

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.|
|enforceComponentsAndStoreApps|1 |Aplicar o componente do Windows e armazenar aplicativos.|
|auditComponentsAndStoreApps|2 |Auditar o componente do Windows e armazenar aplicativos.|
|enforceComponentsStoreAppsAndSmartlocker|3 |Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.|
|auditComponentsStoreAppsAndSmartlocker|4 |Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.|



