---
title: tipo de enumeração resultantAppStateDetail
description: Enum indicando detalhes adicionais sobre por que um aplicativo tem um estado de instalação específico.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 088a84fff9beca407012c8c143f8d58c257d80a9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955607"
---
# <a name="resultantappstatedetail-enum-type"></a>tipo de enumeração resultantAppStateDetail

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Enum indicando detalhes adicionais sobre por que um aplicativo tem um estado de instalação específico.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|noAdditionalDetails|,0|Não há detalhes adicionais disponíveis.|
|dependencyFailedToInstall|1|Uma ou mais dependências do aplicativo não foram instaladas.|
|dependencyWithRequirementsNotMet|duas|Uma ou mais das dependências do aplicativo têm requisitos que não foram atendidos.|
|dependencyPendingReboot|3D|Uma ou mais das dependências do aplicativo exige a reinicialização do dispositivo para concluir a instalação.|
|dependencyWithAutoInstallDisabled|4 |Uma ou mais dependências do aplicativo estão configuradas para não instalar automaticamente.|
|seeInstallErrorCode|2000|Falha ao instalar o aplicativo. Consulte Propriedade de código de erro para obter mais detalhes.|
|autoInstallDisabled|3000|O aplicativo está configurado para não ser instalado automaticamente.|
|seeUninstallErrorCode|4000|Falha ao desinstalar o aplicativo. Consulte Propriedade de código de erro para obter mais detalhes.|
|pendingReboot|5000|O dispositivo deve ser reinicializado para concluir a instalação do aplicativo.|
|installingDependencies|5001|Uma ou mais das dependências do aplicativo estão sendo instaladas.|
|contentDownloaded|5002|O conteúdo do aplicativo foi baixado para o dispositivo.|
|powerShellScriptRequirementNotMet|-1013|A regra de requisito de script do PowerShell não foi atendida|
|registryRequirementNotMet|-1012|A regra de requisito do registro não foi atendida|
|fileSystemRequirementNotMet|-1011|A regra de requisito do sistema de arquivos não foi atendida|
|platformNotApplicable|-1006|O aplicativo não se aplica a esta plataforma. (por exemplo, aplicativo Android direcionado para IOS)|
|minimumCpuSpeedNotMet|-1005|A velocidade da CPU no dispositivo de destino é menor do que o mínimo configurado.|
|minimumLogicalProcessorCountNotMet|-1004|A contagem de processadores lógicos no dispositivo de destino é menor do que o mínimo configurado.|
|minimumPhysicalMemoryNotMet|-1003|A quantidade de RAM no dispositivo de destino é menor do que o mínimo configurado.|
|minimumOsVersionNotMet|-1002|A versão do sistema operacional no dispositivo de destino é menor do que o mínimo configurado.|
|minimumDiskSpaceNotMet|-1001|O espaço em disco disponível no dispositivo de destino é menor do que o mínimo configurado.|
|processorArchitectureNotApplicable|-1000|A arquitetura do dispositivo (por exemplo, x86/AMD64) não se aplica ao aplicativo.|



