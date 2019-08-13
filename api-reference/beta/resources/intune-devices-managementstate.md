---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a61b9d228589f1d0a1e380ed45720f66faa650af
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372150"
---
# <a name="managementstate-enum-type"></a>tipo de enumeração ManagementState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de gerenciamento do dispositivo no Microsoft Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Managed|,0|O dispositivo está sob gerenciamento|
|retirePending|1|Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento|
|retireFailed|duas|Falha no comando de desativação no dispositivo|
|wipePending|3D|Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento|
|wipeFailed|quatro|Falha no comando apagar no dispositivo|
|íntegro|0,5|O dispositivo não está íntegro.|
|deletePending|6|Um comando delete está ocorrendo no dispositivo |
|retireIssued|178|Um comando de retirada foi emitido para o dispositivo|
|wipeIssued|8 |Um comando de apagamento foi emitido para o dispositivo|
|wipeCanceled|9 |Um comando de apagamento para este dispositivo foi cancelado|
|retireCanceled|10 |Um comando de desativação para este dispositivo foi cancelado|
|recém-descobertas|11|O dispositivo é descoberto, mas não está totalmente inscrito.|



