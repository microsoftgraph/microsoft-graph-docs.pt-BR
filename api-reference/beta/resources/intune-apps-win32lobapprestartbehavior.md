---
title: tipo de enumeração win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6747b9b0b3f46e5c2fcf913725d915232a1559ed
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538543"
---
# <a name="win32lobapprestartbehavior-enum-type"></a>tipo de enumeração win32LobAppRestartBehavior

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de ação de reinicialização.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|basedOnReturnCode|,0|O Intune reiniciará o dispositivo após a execução da instalação do aplicativo, se a operação retornar um código de reinicialização.|
|permitiu|1|O Intune não realizará nenhuma ação específica em códigos de reinicialização resultantes de instalações de aplicativos. O Intune não tentará suprimir as reinicializações para os aplicativos MSI.|
|eliminação|duas|O Intune tentará suprimir as reinicializações para os aplicativos MSI.|
|vigor|3D|O Intune forçará o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.|



