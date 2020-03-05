---
title: tipo de enumeração diagnosticDataSubmissionMode
description: Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2d2cc8c0705826015db58ab184b8a499fa2b9c00
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530104"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>tipo de enumeração diagnosticDataSubmissionMode

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Permitir que o dispositivo envie dados de telemetria e diagnósticos de uso, como Watson.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Permite que o usuário defina.|
|nenhuma|1 |Nenhum dado de telemetria é enviado dos componentes do sistema operacional. Observação: esse valor só é aplicável a dispositivos corporativos e de servidor. O uso dessa configuração em outros dispositivos equivale a definir o valor 1.|
|Basic|2 |Envia dados básicos de telemetria.|
|metarquivo|3 |Envia dados de telemetria avançados, incluindo dados de uso e insights.|
|cheia|4 |Envia dados de telemetria completos, incluindo dados de diagnóstico, como o estado do sistema.|



