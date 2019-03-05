---
title: tipo de enumeração resultantAppStateDetail
description: Enum indicando detalhes adicionais sobre por que um aplicativo tem um estado de instalação específico.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d6b7e6a665229d02033cd1c0c25469a83dfc37d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167211"
---
# <a name="resultantappstatedetail-enum-type"></a>tipo de enumeração resultantAppStateDetail

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Enum indicando detalhes adicionais sobre por que um aplicativo tem um estado de instalação específico.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|noAdditionalDetails|,0|Não há detalhes adicionais disponíveis.|
|seeInstallErrorCode|2000|Falha ao instalar o aplicativo. Consulte Propriedade de código de erro para obter mais detalhes.|
|seeUninstallErrorCode|4000|Falha ao desinstalar o aplicativo. Consulte Propriedade de código de erro para obter mais detalhes.|
|pendingReboot|5000|O dispositivo deve ser reinicializado para concluir a instalação do aplicativo.|
|platformNotApplicable|-1006|O aplicativo não se aplica a esta plataforma. (por exemplo, aplicativo Android direcionado para IOS)|
|minimumCpuSpeedNotMet|-1005|A velocidade da CPU no dispositivo de destino é menor do que o mínimo configurado.|
|minimumLogicalProcessorCountNotMet|-1004|A contagem de processadores lógicos no dispositivo de destino é menor do que o mínimo configurado.|
|minimumPhysicalMemoryNotMet|-1003|A quantidade de RAM no dispositivo de destino é menor do que o mínimo configurado.|
|minimumOsVersionNotMet|-1002|A versão do sistema operacional no dispositivo de destino é menor do que o mínimo configurado.|
|minimumDiskSpaceNotMet|-1001|O espaço em disco disponível no dispositivo de destino é menor do que o mínimo configurado.|
|processorArchitectureNotApplicable|-1000|A arquitetura do dispositivo (por exemplo, x86/AMD64) não se aplica ao aplicativo.|




