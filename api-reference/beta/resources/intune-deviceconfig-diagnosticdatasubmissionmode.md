---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ba90c6cbbd8e242e4cd5902a938d5e670d7d2d7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946872"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>tipo de enumeração diagnosticDataSubmissionMode

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Permite que o usuário defina.|
|none|1|Nenhum dado de telemetria é enviado dos componentes do sistema operacional. Observação: esse valor só é aplicável a dispositivos corporativos e de servidor. O uso dessa configuração em outros dispositivos equivale a definir o valor 1.|
|Basic|duas|Envia dados básicos de telemetria.|
|metarquivo|3D|Envia dados de telemetria avançados, incluindo dados de uso e insights.|
|cheia|quatro|Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.|




