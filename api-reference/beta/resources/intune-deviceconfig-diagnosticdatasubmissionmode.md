---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5c1a9e22be20c06b92201dae2b29c43b48166ffe
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791972"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>tipo de enumeração diagnosticDataSubmissionMode

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Permite que o usuário defina.|
|none|1|Nenhum dado de telemetria é enviado dos componentes do sistema operacional. Observação: esse valor só é aplicável a dispositivos corporativos e de servidor. O uso dessa configuração em outros dispositivos equivale a definir o valor 1.|
|Basic|duas|Envia dados básicos de telemetria.|
|metarquivo|3D|Envia dados de telemetria avançados, incluindo dados de uso e insights.|
|cheia|4 |Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.|



