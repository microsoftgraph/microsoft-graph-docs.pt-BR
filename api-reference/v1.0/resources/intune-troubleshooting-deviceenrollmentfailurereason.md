---
title: tipo de enum deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para o registro.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: efee4e4655d36e7575df9e0ddda508dbbcc473c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962069"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>tipo de enum deviceEnrollmentFailureReason

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Categorias de falha de nível superior para o registro.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|0|Valor padrão, o motivo da falha é desconhecido.|
|autenticação|1|Falha na autenticação|
|autorização|2|Chamada foi autenticada, mas não autorizada a registrar.|
|accountValidation|3|Falha ao validar a conta para o registro. (Conta bloqueada, o registro não habilitado)|
|userValidation|4|Usuário não pôde ser validado. (Usuário não existe, licença falta)|
|deviceNotSupported|5|Não há suporte para o dispositivo para gerenciamento de dispositivos móveis.|
|inMaintenance|6|Conta está na manutenção.|
|badRequest|7|Cliente enviou uma solicitação que não seja compreendidos/suportados pelo serviço.|
|featureNotSupported|8|Os recursos usados por esta inscrição não são suportados para essa conta.|
|enrollmentRestrictionsEnforced|9|Restrições de registro configuradas pelo administrador bloqueado este registro.|
|clientDisconnected|10|Cliente esgotado ou inscrição foi anulada pelo usuário final.|
|userAbandonment|11|O registro foi abandonado pelo usuário final. (Usuário final inclusão de Introdução, mas não conseguiu concluí-la no modo oportuno)|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->
