---
title: tipo de enum remoteAction
description: Ações remotas Intune oferece suporte.
author: tfitzmac
ms.openlocfilehash: 7b301757ec5bb8c9c9a0336cbc83d6a458579916
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362556"
---
# <a name="remoteaction-enum-type"></a>tipo de enum remoteAction

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ações remotas Intune oferece suporte.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|0|Usuário inicia uma ação desconhecida.|
|factoryReset|1|Usuário inicia uma ação à fábrica reiniciar um dispositivo. |
|removeCompanyData|2|Usuário inicia uma ação para remover os dados da empresa de um dispositivo. |
|resetPasscode|3|Usuário inicia uma ação para remover a senha de um dispositivo iOS ou redefinir a senha do Android / dispositivo do Windows. |
|remoteLock|4|Usuário inicia uma ação para bloqueio remoto um dispositivo.|
|enableLostMode|5|Usuário inicia uma ação para habilitar o modo perdido em um dispositivo iOS supervisionadas.|
|disableLostMode|6|Usuário inicia uma ação para desativar o modo perdido em um dispositivo iOS supervisionadas.|
|locateDevice|7|Usuário inicia uma ação para localizar um dispositivo iOS supervisionadas.|
|rebootNow|8|Usuário inicia uma ação para reinicializar um dispositivo do Windows.|
|recoverPasscode|9|Usuário inicia uma ação para redefinir o pin para passport para trabalhar no dispositivo do windows phone.|
|cleanWindowsDevice|10|Usuário inicia uma ação para limpar o dispositivo do windows.|
|logoutSharedAppleDeviceActiveUser|11|Usuário inicia uma ação para logoff do usuário atual no dispositivo apple compartilhado.|
|quickScan|12|Usuário inicia uma ação para executar a verificação rápida no dispositivo.|
|fullScan|13|Usuário inicia uma ação para executar a verificação completa no dispositivo.|
|windowsDefenderUpdateSignatures|14|Usuário inicia uma ação para atualizar as assinaturas de malware no dispositivo.|
|factoryResetKeepEnrollmentData|15|Usuário inicia um dispositivo de apagamento remoto de ação com mantendo os dados de inscrição.|
|updateDeviceAccount|16|Usuário inicia uma ação para atualizar a conta no dispositivo.|
|automaticRedeployment|17|Usuário inicia uma ação para o dispositivo de reimplantação de automatice|
|Desligamento|18|Usuário inicia uma ação para desligar o dispositivo.|





