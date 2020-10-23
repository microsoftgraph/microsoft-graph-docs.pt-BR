---
title: tipo de enumeração remoteaction
description: As ações remotas do Intune dão suporte.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6f0d1fb60610425356f543d884e311d041a441cb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725418"
---
# <a name="remoteaction-enum-type"></a>tipo de enumeração remoteaction

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

As ações remotas do Intune dão suporte.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O usuário inicia uma ação desconhecida.|
|factoryReset|1|O usuário inicia uma ação para a redefinição de fábrica de um dispositivo. |
|removeCompanyData|duas|O usuário inicia uma ação para remover dados da empresa de um dispositivo. |
|resetPasscode|3D|O usuário inicia uma ação para remover a senha de um dispositivo iOS ou redefinir a senha do dispositivo Android/Windows. |
|remoteLock|4 |O usuário inicia uma ação para bloquear remotamente um dispositivo.|
|enableLostMode|5 |O usuário inicia uma ação para habilitar o modo perdido em um dispositivo iOS supervisionado.|
|disableLostMode|6 |O usuário inicia uma ação para desabilitar o modo perdido em um dispositivo iOS supervisionado.|
|locateDevice|7 |O usuário inicia uma ação para localizar um dispositivo iOS supervisionado.|
|rebootNow|8 |O usuário inicia uma ação para reinicializar um dispositivo Windows.|
|recoverPasscode|9 |O usuário inicia uma ação para redefinir o PIN para o Passport para funcionar no dispositivo Windows Phone.|
|cleanWindowsDevice|10 |O usuário inicia uma ação para limpar o dispositivo Windows.|
|logoutSharedAppleDeviceActiveUser|11|O usuário inicia uma ação para fazer o logoff do usuário atual em um dispositivo Apple compartilhado.|
|quickScan|12 |O usuário inicia uma ação para executar a verificação rápida no dispositivo.|
|fullScan|13 |O usuário inicia uma ação para executar a verificação completa no dispositivo.|
|windowsDefenderUpdateSignatures|14 |O usuário inicia uma ação para atualizar as assinaturas de malware no dispositivo.|
|factoryResetKeepEnrollmentData|15 |O usuário inicia um dispositivo de apagamento remoto de ação com a manutenção dos dados de registro.|
|updateDeviceAccount|16 |O usuário inicia uma ação para atualizar a conta no dispositivo.|
|automaticRedeployment|17 |O usuário inicia uma ação para automático reimplantar o dispositivo|
|Parada|18 |O usuário inicia uma ação para desligar o dispositivo.|
|rotateBitLockerKeys|19|O usuário inicia uma ação para girar o BitLockerKeys no dispositivo.|
|rotateFileVaultKey|508|O usuário inicia uma ação para girar o FileVaultKey no Mac.|
|getFileVaultKey| 21 |O usuário inicia uma ação para obter o FileVaultKey no Mac.|
|DeviceName|22|O usuário inicia uma ação para definir o nome do dispositivo no dispositivo.|





