---
title: tipo denum resultantAppStateDetail
description: Enum indicando detalhes adicionais sobre por que um aplicativo tem um estado de instalação específico.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4b83040763f0b7b56c4a6e8979a06f3f945a39ed94dde254c042648f8fe349f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54250060"
---
# <a name="resultantappstatedetail-enum-type"></a>tipo denum resultantAppStateDetail

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Enum indicando detalhes adicionais sobre por que um aplicativo tem um estado de instalação específico.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|noAdditionalDetails|0|Nenhum detalhe adicional está disponível.|
|dependencyFailedToInstall|1 |Uma ou mais dependências do aplicativo falharam na instalação.|
|dependencyWithRequirementsNotMet|2|Uma ou mais dependências do aplicativo têm requisitos que não são atendidos.|
|dependencyPendingReboot|3 |Uma ou mais dependências do aplicativo exigem uma reinicialização do dispositivo para concluir a instalação.|
|dependencyWithAutoInstallDisabled|4 |Uma ou mais dependências do aplicativo são configuradas para não instalar automaticamente.|
|iosAppStoreUpdateFailedToInstall|1000|A versão mais recente do aplicativo falhou ao atualizar de uma versão anterior.|
|vppAppHasUpdateAvailable|1001|Uma atualização está disponível.|
|userRejectedUpdate|1002|O usuário rejeitou a atualização do aplicativo. |
|seeInstallErrorCode|2000|Falha na instalação do aplicativo. Consulte a propriedade de código de erro para obter mais detalhes.|
|autoInstallDisabled|3000|O aplicativo está configurado para não ser instalado automaticamente.|
|managedAppNoLongerPresent|3001|O aplicativo é gerenciado, mas não é mais instalado.|
|userRejectedInstall|3002|O usuário rejeitou a instalação do aplicativo.|
|userIsNotLoggedIntoAppStore|3003|O usuário deve fazer logoff na App Store para instalar o aplicativo.|
|seeUninstallErrorCode|4000|Falha ao desinstalar o aplicativo. Consulte a propriedade de código de erro para obter mais detalhes.|
|pendingReboot|5000|O dispositivo deve ser reiniciado para concluir a instalação do aplicativo.|
|installingDependencies|5001|Uma ou mais dependências do aplicativo estão sendo instaladas.|
|contentDownloaded|5002|O conteúdo do aplicativo foi baixado para o dispositivo.|
|powerShellScriptRequirementNotMet|-1013|A regra de requisito de script do PowerShell não é atendida|
|registryRequirementNotMet|-1012|Regra de requisitos do Registro não é atendida|
|fileSystemRequirementNotMet|-1011|A regra de requisito do sistema de arquivos não é atendida|
|platformNotApplicable|-1006|O aplicativo não é aplicável a essa plataforma. (por exemplo, aplicativo Android direcionado para IOS)|
|minimumCpuSpeedNotMet|-1005|A velocidade da CPU no dispositivo de destino é menor do que o mínimo configurado.|
|minimumLogicalProcessorCountNotMet|-1004|A contagem de processadores lógicos no dispositivo de destino é menor do que o mínimo configurado.|
|minimumPhysicalMemoryNotMet|-1003|A quantidade de RAM no dispositivo de destino é menor do que o mínimo configurado.|
|minimumOsVersionNotMet|-1002|A versão do sistema operacional no dispositivo de destino é menor do que o mínimo configurado.|
|minimumDiskSpaceNotMet|-1001|O espaço em disco disponível no dispositivo de destino é menor do que o mínimo configurado.|
|processorArchitectureNotApplicable|-1000|A arquitetura do dispositivo (por exemplo, x86/amd64) não é aplicável para o aplicativo.|




