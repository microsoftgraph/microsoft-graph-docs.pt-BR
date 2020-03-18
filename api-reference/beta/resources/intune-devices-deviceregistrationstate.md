---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 908f38a2da8f5960eb9c5f1879b7b54374b806ed
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784130"
---
# <a name="deviceregistrationstate-enum-type"></a>tipo de enumeração deviceRegistrationState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status do registro do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Não registrado|,0|O dispositivo não está registrado.|
|inscreve|duas|O dispositivo está registrado.|
|revogado|3D|O dispositivo foi bloqueado, apagado ou desativado.|
|keyconflict|4 |O dispositivo tem um conflito de teclas.|
|approvalPending|5 |O dispositivo está aguardando aprovação.|
|certificateReset|6 |O certificado de dispositivo foi redefinido.|
|notRegisteredPendingEnrollment|7 |O dispositivo não está registrado e registro pendente.|
|desconhecido|8 |O status do registro do dispositivo é desconhecido.|



