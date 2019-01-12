---
title: tipo de enum diagnosticDataSubmissionMode
description: Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a293288c3891f8ecd77d422986e419d2e3d53767
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912943"
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



