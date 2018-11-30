---
title: tipo de enum diagnosticDataSubmissionMode
description: Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.
ms.openlocfilehash: b09a4bf334af5981c3ce6dabbab0ac64e2b24887
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006494"
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



