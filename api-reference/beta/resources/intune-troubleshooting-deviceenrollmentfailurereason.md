---
title: tipo de enumeração deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para registro.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f03ce73f1d6f8b5edc6b3e3b661f9a7ba79407bb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163851"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>tipo de enumeração deviceEnrollmentFailureReason

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Categorias de falha de nível superior para registro.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|,0|O valor padrão, motivo da falha é desconhecido.|
|autentica|1|Falha de autenticação|
|nesse|duas|A chamada foi autenticada, mas não está autorizada a se inscrever.|
|accountValidation|3D|Falha ao validar a conta para registro. (Conta bloqueada, registro não habilitado)|
|userValidation|quatro|Não foi possível validar o usuário. (O usuário não existe, licença ausente)|
|deviceNotSupported|0,5|O dispositivo não tem suporte para gerenciamento de dispositivos móveis.|
|inManutenção|6|A conta está em manutenção.|
|badRequest|178|O cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.|
|featureNotSupported|8|Não há suporte para os recursos usados por este registro para esta conta.|
|enrollmentRestrictionsEnforced|241|As restrições de registro configuradas pelo administrador bloquearam esse registro.|
|clientDisconnected|254|O cliente esgotou o tempo limite ou o registro foi anulado pelo enduser.|
|Membrouserabandonment|11|O registro foi abandonado pelo enduser. (Enduser Started onboard, mas não conseguiu concluí-la na forma oportuna)|




