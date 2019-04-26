---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580971"
---
# <a name="deviceregistrationstate-enum-type"></a>tipo de enumeração deviceRegistrationState

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status do registro do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Não registrado|,0|O dispositivo não está registrado.|
|inscreve|2 |O dispositivo está registrado.|
|revogado|3 |O dispositivo foi bloqueado, apagado ou desativado.|
|keyConflict|4 |O dispositivo tem um conflito de teclas.|
|approvalPending|5 |O dispositivo está aguardando aprovação.|
|certificateReset|6 |O certificado de dispositivo foi redefinido.|
|notRegisteredPendingEnrollment|7 |O dispositivo não está registrado e registro pendente.|
|desconhecido|8 |O status do registro do dispositivo é desconhecido.|



