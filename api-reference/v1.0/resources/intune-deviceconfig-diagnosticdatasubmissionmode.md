---
title: tipo de enum diagnosticDataSubmissionMode
description: Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.
localization_priority: Normal
ms.openlocfilehash: 1654e9c5c94fd79bbda0d77ef84101fb9fb92d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812779"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>tipo de enum diagnosticDataSubmissionMode

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Permitir que o usuário pode definir.|
|nenhum|1|Nenhum dado de telemetria é enviado de componentes do sistema operacional. Observação: Esse valor só é aplicável aos dispositivos enterprise e servidor. O uso dessa configuração em outros dispositivos é equivalente a definir o valor de 1.|
|básico|2|Envia dados de Telemetria básica.|
|Avançado|3|Envia aprimorado de dados de telemetria, incluindo dados de uso e ideias.|
|completo|4|Envia dados de telemetria completo incluindo dados de diagnósticos, como o estado do sistema.|



