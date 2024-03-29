---
title: Tipo de número remoteAction
description: Ações remotas Compatíveis com o Intune.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 70e7d5ac0734f791f79915524565012393b6f90d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081084"
---
# <a name="remoteaction-enum-type"></a>Tipo de número remoteAction

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ações remotas Compatíveis com o Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|O usuário inicia uma ação desconhecida.|
|factoryReset|1|O usuário inicia uma ação para redefinir de fábrica um dispositivo. |
|removeCompanyData|2|O usuário inicia uma ação para remover dados da empresa de um dispositivo. |
|resetPasscode|3|O usuário inicia uma ação para remover a senha de um dispositivo iOS ou redefinir a senha do dispositivo Android/Windows. |
|remoteLock|4 |O usuário inicia uma ação para bloquear um dispositivo remotamente.|
|enableLostMode|5 |O usuário inicia uma ação para habilitar o modo perdido em um dispositivo iOS supervisionado.|
|disableLostMode|6 |O usuário inicia uma ação para desabilitar o modo perdido em um dispositivo iOS supervisionado.|
|locateDevice|7 |O usuário inicia uma ação para localizar um dispositivo iOS supervisionado.|
|rebootNow|8 |O usuário inicia uma ação para reiniciar um Windows dispositivo.|
|recoverPasscode|9 |O usuário inicia uma ação para redefinir o pino para o passport para trabalho no dispositivo windows phone.|
|cleanWindowsDevice|10 |O usuário inicia uma ação para limpar o dispositivo windows.|
|logoutSharedAppleDeviceActiveUser|11|O usuário inicia uma ação para fazer logoff do usuário atual no dispositivo apple compartilhado.|
|quickScan|12 |O usuário inicia uma ação para executar uma verificação rápida no dispositivo.|
|fullScan|13|O usuário inicia uma ação para executar a verificação completa no dispositivo.|
|windowsDefenderUpdateSignatures|14 |O usuário inicia uma ação para atualizar assinaturas de malware no dispositivo.|
|factoryResetKeepEnrollmentData|15 |O usuário inicia um dispositivo de limpeza remota de ação com a manutenção de dados de registro.|
|updateDeviceAccount|16 |O usuário inicia uma ação para atualizar a conta no dispositivo.|
|automaticRedeployment|17 |O usuário inicia uma ação para reimplantar automaticamente o dispositivo|
|shutDown|18 |O usuário inicia uma ação para desligar o dispositivo.|
|rotateBitLockerKeys|19|O usuário inicia uma ação para Girar BitLockerKeys no dispositivo.|
|rotateFileVaultKey|20|O usuário inicia uma ação para Girar FileVaultKey no mac.|
|getFileVaultKey| 21 |O usuário inicia uma ação para Obter FileVaultKey no mac.|
|setDeviceName|22|O usuário inicia uma ação para definir o Nome do Dispositivo no dispositivo.|
|activateDeviceEsim|23|O usuário inicia uma ação para ativar o eSIM no dispositivo.|



