---
title: tipo de enumeração win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9632b0199fc3bdc659f4c94fe71311ad2e896ce8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49284558"
---
# <a name="win32lobapprestartbehavior-enum-type"></a>tipo de enumeração win32LobAppRestartBehavior

Namespace: microsoft.graph

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




