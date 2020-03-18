---
title: tipo de enumeração win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 16fda1d530614ea138ecc575930b4800b5f143c4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797553"
---
# <a name="win32lobapprestartbehavior-enum-type"></a>tipo de enumeração win32LobAppRestartBehavior

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de ação de reinicialização.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|basedOnReturnCode|,0|O Intune reiniciará o dispositivo após a execução da instalação do aplicativo, se a operação retornar um código de reinicialização.|
|permitiu|1|O Intune não realizará nenhuma ação específica em códigos de reinicialização resultantes de instalações de aplicativos. O Intune não tentará suprimir as reinicializações para os aplicativos MSI.|
|eliminação|duas|O Intune tentará suprimir as reinicializações para os aplicativos MSI.|
|vigor|3D|O Intune forçará o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.|



