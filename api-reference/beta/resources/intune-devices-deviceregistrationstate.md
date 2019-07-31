---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e153ac5c1bfbd09540fd55b5df23eab095e2a002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968383"
---
# <a name="deviceregistrationstate-enum-type"></a>tipo de enumeração deviceRegistrationState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status do registro do dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Não registrado|,0|O dispositivo não está registrado.|
|inscreve|duas|O dispositivo está registrado.|
|revogado|3D|O dispositivo foi bloqueado, apagado ou desativado.|
|keyconflict|quatro|O dispositivo tem um conflito de teclas.|
|approvalPending|0,5|O dispositivo está aguardando aprovação.|
|certificateReset|6|O certificado de dispositivo foi redefinido.|
|notRegisteredPendingEnrollment|178|O dispositivo não está registrado e registro pendente.|
|desconhecido|8 |O status do registro do dispositivo é desconhecido.|





