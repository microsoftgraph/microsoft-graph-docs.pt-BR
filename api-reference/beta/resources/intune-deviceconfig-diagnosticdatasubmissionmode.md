---
title: tipo de enum diagnosticDataSubmissionMode
description: Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b587d6872bcd3610c3b878ae7a672c3e776ea01
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422254"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>tipo de enum diagnosticDataSubmissionMode

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Permitir que o usuário pode definir.|
|none|1|Nenhum dado de telemetria é enviado de componentes do sistema operacional. Observação: Esse valor só é aplicável aos dispositivos enterprise e servidor. O uso dessa configuração em outros dispositivos é equivalente a definir o valor de 1.|
|básico|2|Envia dados de Telemetria básica.|
|Avançado|3|Envia aprimorado de dados de telemetria, incluindo dados de uso e ideias.|
|completo|4|Envia dados de telemetria completo incluindo dados de diagnósticos, como o estado do sistema.|




