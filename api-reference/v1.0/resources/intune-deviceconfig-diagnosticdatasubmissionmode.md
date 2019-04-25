---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c0707b97e60da406210d6a091ed0dd4efaa2299
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578019"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>tipo de enumeração diagnosticDataSubmissionMode

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|,0|Permite que o usuário defina.|
|Nenhuma|1 |Nenhum dado de telemetria é enviado dos componentes do sistema operacional. Observação: esse valor só é aplicável a dispositivos corporativos e de servidor. O uso dessa configuração em outros dispositivos equivale a definir o valor 1.|
|Basic|2 |Envia dados básicos de telemetria.|
|metarquivo|3 |Envia dados de telemetria avançados, incluindo dados de uso e insights.|
|cheia|4 |Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.|



