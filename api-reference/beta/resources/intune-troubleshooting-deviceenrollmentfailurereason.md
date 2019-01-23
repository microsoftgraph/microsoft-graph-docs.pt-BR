---
title: tipo de enum deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para o registro.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fbfe7193c72f1ff1a03a7e7bb4da57d0a032e530
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396207"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>tipo de enum deviceEnrollmentFailureReason

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




