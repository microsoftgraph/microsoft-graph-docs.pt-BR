---
title: tipo de enumeração deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para registro.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: efe1a63a86a01001168d2d631280e8a190125987
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368047"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>tipo de enumeração deviceEnrollmentFailureReason

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Categorias de falha de nível superior para registro.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O valor padrão, motivo da falha é desconhecido.|
|autentica|1|Falha de autenticação|
|nesse|duas|A chamada foi autenticada, mas não está autorizada a se inscrever.|
|accountValidation|3D|Falha ao validar a conta para registro. (Conta bloqueada, registro não habilitado)|
|uservalidation|quatro|Não foi possível validar o usuário. (O usuário não existe, licença ausente)|
|deviceNotSupported|0,5|O dispositivo não tem suporte para gerenciamento de dispositivos móveis.|
|inmanutenção|6|A conta está em manutenção.|
|badRequest|178|O cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.|
|featureNotSupported|8 |Não há suporte para os recursos usados por este registro para esta conta.|
|enrollmentRestrictionsEnforced|9 |As restrições de registro configuradas pelo administrador bloquearam esse registro.|
|clientDisconnected|10 |O cliente esgotou o tempo limite ou o registro foi anulado pelo enduser.|
|Membrouserabandonment|11|O registro foi abandonado pelo enduser. (Enduser Started onboard, mas não conseguiu concluí-la na forma oportuna)|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->


