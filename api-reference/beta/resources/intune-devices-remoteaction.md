---
title: tipo de enum remoteAction
description: Ações remotas Intune oferece suporte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3177ea43599cd155e11af1786636111a8578d29b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405538"
---
# <a name="remoteaction-enum-type"></a>tipo de enum remoteAction

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




