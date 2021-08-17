---
title: Tipo de número deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para registro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7f47c4903c17d8c99408449d32b83a38a7389204
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266804"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>Tipo de número deviceEnrollmentFailureReason

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Categorias de falha de nível superior para registro.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Valor padrão, motivo da falha é desconhecido.|
|authentication|1 |Falha na autenticação|
|authorization|2|A chamada foi autenticada, mas não autorizada a se inscrever.|
|accountValidation|3 |Falha ao validar a conta para registro. (Conta bloqueada, registro não habilitado)|
|userValidation|4 |O usuário não pôde ser validado. (O usuário não existe, licença ausente)|
|deviceNotSupported|5 |Não há suporte para o gerenciamento de dispositivos móveis.|
|inMaintenance|6 |A conta está em manutenção.|
|badRequest|7 |O cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.|
|featureNotSupported|8 |Os recursos usados por esse registro não são suportados para essa conta.|
|enrollmentRestrictionsEnforced|9 |As restrições de registro configuradas pelo administrador bloquearam esse registro.|
|clientDisconnected|10 |O tempo de término do cliente ou o registro foi abortado pelo usuário final.|
|userAbandonment|11 |O registro foi abandonado pelo usuário final. (O Usuário final começou a integração, mas falhou ao concluí-lo em tempo hábil)|




