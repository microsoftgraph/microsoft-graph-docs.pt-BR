---
title: tipo de enumeração remoteaction
description: As ações remotas do Intune dão suporte.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ad0666ffc94fcfdc09e289dde80f178e92f09af
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941825"
---
# <a name="remoteaction-enum-type"></a>tipo de enumeração remoteaction

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

As ações remotas do Intune dão suporte.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O usuário inicia uma ação desconhecida.|
|factoryReset|1|O usuário inicia uma ação para a redefinição de fábrica de um dispositivo. |
|removeCompanyData|duas|O usuário inicia uma ação para remover dados da empresa de um dispositivo. |
|resetPasscode|3D|O usuário inicia uma ação para remover a senha de um dispositivo iOS ou redefinir a senha do dispositivo Android/Windows. |
|remoteLock|quatro|O usuário inicia uma ação para bloquear remotamente um dispositivo.|
|enableLostMode|0,5|O usuário inicia uma ação para habilitar o modo perdido em um dispositivo iOS supervisionado.|
|disableLostMode|6|O usuário inicia uma ação para desabilitar o modo perdido em um dispositivo iOS supervisionado.|
|locateDevice|178|O usuário inicia uma ação para localizar um dispositivo iOS supervisionado.|
|rebootNow|8 |O usuário inicia uma ação para reinicializar um dispositivo Windows.|
|recoverPasscode|9 |O usuário inicia uma ação para redefinir o PIN para o Passport para funcionar no dispositivo Windows Phone.|
|cleanWindowsDevice|10 |O usuário inicia uma ação para limpar o dispositivo Windows.|
|logoutSharedAppleDeviceActiveUser|11|O usuário inicia uma ação para fazer o logoff do usuário atual em um dispositivo Apple compartilhado.|
|quickScan|3,6|O usuário inicia uma ação para executar a verificação rápida no dispositivo.|
|fullScan|Treze|O usuário inicia uma ação para executar a verificação completa no dispositivo.|
|windowsDefenderUpdateSignatures|14|O usuário inicia uma ação para atualizar as assinaturas de malware no dispositivo.|
|factoryResetKeepEnrollmentData|15|O usuário inicia um dispositivo de apagamento remoto de ação com a manutenção dos dados de registro.|
|updateDeviceAccount|dezesseis|O usuário inicia uma ação para atualizar a conta no dispositivo.|
|automaticRedeployment|17.07.06|O usuário inicia uma ação para automático reimplantar o dispositivo|
|Parada|anos|O usuário inicia uma ação para desligar o dispositivo.|




