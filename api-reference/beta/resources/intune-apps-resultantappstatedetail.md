---
title: tipo de enum resultantAppStateDetail
description: Enum indicando maiores detalhes sobre por que um aplicativo tem um determinado estado de instalação.
author: tfitzmac
ms.openlocfilehash: e06e8afb6ebb5e22abf11d9cd53150bed5288052
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352525"
---
# <a name="resultantappstatedetail-enum-type"></a>tipo de enum resultantAppStateDetail

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Enum indicando maiores detalhes sobre por que um aplicativo tem um determinado estado de instalação.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|noAdditionalDetails|0|Sem detalhes adicionais estão disponíveis.|
|seeInstallErrorCode|2000|Falha ao instalar o aplicativo. Consulte a propriedade de código de erro para obter mais detalhes.|
|seeUninstallErrorCode|4000|Falha ao desinstalar o aplicativo. Consulte a propriedade de código de erro para obter mais detalhes.|
|pendingReboot|5000|Dispositivo deve ser reiniciado para concluir a instalação do aplicativo.|
|platformNotApplicable|-1006|Aplicativo não é aplicável a nesta plataforma. (por exemplo, Android app voltada para o IOS)|
|minimumCpuSpeedNotMet|-1005|Velocidade da CPU no dispositivo de destino é menor que o mínimo configurado.|
|minimumLogicalProcessorCountNotMet|-1004|Contagem de processadores lógicos no dispositivo de destino é menor que o mínimo configurado.|
|minimumPhysicalMemoryNotMet|-1003|Quantidade de RAM no dispositivo de destino é menor que o mínimo configurado.|
|minimumOsVersionNotMet|-1002|Versão do sistema operacional no dispositivo de destino é menor que o mínimo configurado.|
|minimumDiskSpaceNotMet|-1001|Espaço em disco disponível no dispositivo de destino é menor que o mínimo configurado.|
|processorArchitectureNotApplicable|-1000|Arquitetura de dispositivo (ex.: x86/amd64) não é aplicável para o aplicativo.|





