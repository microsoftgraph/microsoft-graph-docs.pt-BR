---
title: Tipo de número managementState
description: Estado de gerenciamento do dispositivo Microsoft Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 814395189273adfe7a977ddb2d85e6ed8714aa64
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796583"
---
# <a name="managementstate-enum-type"></a>Tipo de número managementState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de gerenciamento do dispositivo Microsoft Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|managed|0|O dispositivo está sob gerenciamento|
|retirePending|1|Um comando retire está ocorrendo no dispositivo e no processo de desemrolling do gerenciamento|
|retireFailed|2|Falha no comando Retire no dispositivo|
|wipePending|3|Um comando wipe está ocorrendo no dispositivo e no processo de desemrolling do gerenciamento|
|wipeFailed|4 |Falha no comando Wipe no dispositivo|
|unhealthy|5 |O dispositivo não está 100%.|
|deletePending|6 |Um comando delete está ocorrendo no dispositivo |
|retireIssued|7 |Um comando retire foi emitido para o dispositivo|
|wipeIssued|8 |Um comando wipe foi emitido para o dispositivo|
|wipeCanceled|9 |Um comando wipe para este dispositivo foi cancelado|
|retireCanceled|10 |Um comando retire para este dispositivo foi cancelado|
|discovered|11 |O dispositivo é descoberto, mas não está totalmente inscrito.|



