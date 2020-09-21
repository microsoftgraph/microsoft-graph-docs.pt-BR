---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7ef0a61e8d95793e6e4717a3a5ed66d518e80590
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968441"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>tipo de enumeração diagnosticDataSubmissionMode

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Permite que o usuário defina.|
|Nenhuma|1 |Nenhum dado de telemetria é enviado dos componentes do sistema operacional. Observação: esse valor só é aplicável a dispositivos corporativos e de servidor. O uso dessa configuração em outros dispositivos equivale a definir o valor 1.|
|Basic|2 |Envia dados básicos de telemetria.|
|metarquivo|3 |Envia dados de telemetria avançados, incluindo dados de uso e insights.|
|cheia|4 |Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.|






