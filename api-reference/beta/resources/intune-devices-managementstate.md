---
title: tipo de enum managementState
description: Estado de gerenciamento de dispositivo no Microsoft Intune.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8d0801949125f3b0cceb865ac1f8546195112e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420014"
---
# <a name="managementstate-enum-type"></a>tipo de enum managementState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Estado de gerenciamento de dispositivo no Microsoft Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|gerenciados|0|O dispositivo está sob gerenciamento|
|retirePending|1|Um comando de aposentadoria está ocorrendo no dispositivo e no processo de unenrolling de gerenciamento|
|retireFailed|2|Desative o comando falha no dispositivo|
|wipePending|3|Um comando de apagamento está ocorrendo no dispositivo e no processo de unenrolling de gerenciamento|
|wipeFailed|4|Falha do comando de apagamento do dispositivo|
|não íntegro|5|O dispositivo não está íntegro.|
|deletePending|6|Um comando Excluir está ocorrendo no dispositivo |
|retireIssued|7|Um comando de aposentadoria foi emitido para o dispositivo|
|wipeIssued|8|Foi emitido um comando de apagamento do dispositivo|
|wipeCanceled|9|Um comando de apagamento para este dispositivo foi cancelado|
|retireCanceled|10|Um comando de aposentadoria para este dispositivo foi cancelado|
|descoberto|11|O dispositivo é descoberto, mas não totalmente registrado.|




