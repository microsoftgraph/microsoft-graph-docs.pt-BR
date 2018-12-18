---
title: tipo de enum deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para o registro.
author: tfitzmac
ms.openlocfilehash: 7747008f00348a4671713a28c0d1e48e156e9b38
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325078"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>tipo de enum deviceEnrollmentFailureReason

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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





