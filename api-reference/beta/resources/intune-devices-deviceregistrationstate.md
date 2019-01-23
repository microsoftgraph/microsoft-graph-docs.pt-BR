---
title: tipo de enum deviceRegistrationState
description: Status do registro do dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90f2dc7f8c11940fa01047d8c61f23c8f0389ed8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396753"
---
# <a name="deviceregistrationstate-enum-type"></a>tipo de enum deviceRegistrationState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Status do registro do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notRegistered|0|O dispositivo não está registrado.|
|registrado|2|O dispositivo está registrado.|
|revogado|3|O dispositivo foi bloqueado, apagado ou desativado.|
|keyConflict|4|O dispositivo tem um conflito de chave.|
|approvalPending|5|O dispositivo está aguardando aprovação.|
|certificateReset|6|O certificado do dispositivo foi redefinido.|
|notRegisteredPendingEnrollment|7|O dispositivo não está registrado e pendentes de inscrição.|
|unknown|8|O status do registro de dispositivo é desconhecido.|




