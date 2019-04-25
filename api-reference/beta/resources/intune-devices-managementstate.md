---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05dc0db1ecbe88616ca36db82bad2081b4133e3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521289"
---
# <a name="managementstate-enum-type"></a>tipo de enumeração ManagementState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de gerenciamento do dispositivo no Microsoft Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Managed|,0|O dispositivo está sob gerenciamento|
|retirePending|1 |Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento|
|retireFailed|2 |Falha no comando de desAtivação no dispositivo|
|wipePending|3 |Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento|
|wipeFailed|4 |Falha no comando apagar no dispositivo|
|íntegro|5 |O dispositivo não está íntegro.|
|deletePending|6 |Um comando delete está ocorrendo no dispositivo |
|retireIssued|7 |Um comando de retirada foi emitido para o dispositivo|
|wipeIssued|8 |Um comando de apagamento foi emitido para o dispositivo|
|wipeCanceled|9 |Um comando de apagamento para este dispositivo foi cancelado|
|retireCanceled|10 |Um comando de desativação para este dispositivo foi cancelado|
|recém-descobertas|11 |O dispositivo é descoberto, mas não está totalmente inscrito.|





