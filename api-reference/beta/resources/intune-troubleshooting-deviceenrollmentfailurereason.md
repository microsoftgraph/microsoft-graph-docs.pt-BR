---
title: tipo de enumeração deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para registro.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0921098dcaa4905b0b7eaf5722acf4edac8419f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558192"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>tipo de enumeração deviceEnrollmentFailureReason

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Categorias de falha de nível superior para registro.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O valor padrão, motivo da falha é desconhecido.|
|autentica|1 |Falha de autenticação|
|nesse|2 |A chamada foi autenticada, mas não está autorizada a se inscrever.|
|accountValidation|3 |Falha ao validar a conta para registro. (Conta bloqueada, registro não habilitado)|
|userValidation|4 |Não foi possível validar o usuário. (O usuário não existe, licença ausente)|
|deviceNotSupported|5 |O dispositivo não tem suporte para gerenciamento de dispositivos móveis.|
|inManutenção|6 |A conta está em manutenção.|
|badRequest|7 |O cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.|
|featureNotSupported|8 |Não há suporte para os recursos usados por este registro para esta conta.|
|enrollmentRestrictionsEnforced|9 |As restrições de registro configuradas pelo administrador bloquearam esse registro.|
|clientDisconnected|10 |O cliente esgotou o tempo limite ou o registro foi anulado pelo enduser.|
|Membrouserabandonment|11 |O registro foi abandonado pelo enduser. (Enduser Started onboard, mas não conseguiu concluí-la na forma oportuna)|



