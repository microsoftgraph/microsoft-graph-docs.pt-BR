---
title: tipo de enumeração win32LobAppRestartBehavior
description: Indica o tipo de ação de reinicialização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 61c41f8e2d9d0b787988a10e0562d10567bf1b64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071049"
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
|permitiu|1 |O Intune não realizará nenhuma ação específica em códigos de reinicialização resultantes de instalações de aplicativos. O Intune não tentará suprimir as reinicializações para os aplicativos MSI.|
|eliminação|2 |O Intune tentará suprimir as reinicializações para os aplicativos MSI.|
|vigor|3 |O Intune forçará o dispositivo a reiniciar imediatamente após a operação de instalação do aplicativo.|






