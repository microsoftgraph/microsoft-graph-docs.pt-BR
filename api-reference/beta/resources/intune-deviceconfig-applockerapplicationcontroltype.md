---
title: tipo de enumeração appLockerApplicationControlType
description: Valores possíveis dos tipos de controle do aplicativo AppLocker
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5455cb2a4e8e16f8bd5ca737655f50f625c3151f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469898"
---
# <a name="applockerapplicationcontroltype-enum-type"></a>tipo de enumeração appLockerApplicationControlType

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis dos tipos de controle do aplicativo AppLocker

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Valor padrão do dispositivo, nenhum tipo de controle do aplicativo selecionado.|
|enforceComponentsAndStoreApps|1|Aplicar o componente do Windows e armazenar aplicativos.|
|auditComponentsAndStoreApps|duas|Auditar o componente do Windows e armazenar aplicativos.|
|enforceComponentsStoreAppsAndSmartlocker|3D|Aplicar componentes do Windows, armazenar aplicativos e armário inteligente.|
|auditComponentsStoreAppsAndSmartlocker|4 |Auditoria de componentes do Windows, aplicativos de armazenamento e armário inteligente.|



