---
title: tipo de enum resultantAppStateDetail
description: Enum indicando maiores detalhes sobre por que um aplicativo tem um determinado estado de instalação.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34b4d885f9ed2a23669bc2e30c91de40af8d915b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410235"
---
# <a name="resultantappstatedetail-enum-type"></a>tipo de enum resultantAppStateDetail

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




