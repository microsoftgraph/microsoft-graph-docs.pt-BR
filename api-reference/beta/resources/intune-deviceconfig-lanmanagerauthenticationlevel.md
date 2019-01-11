---
title: tipo de enum lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68af209a005dc1d7e8d25672f5e97e1d929ba25b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866910"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>tipo de enum lanManagerAuthenticationLevel

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para LanManagerAuthenticationLevel
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|lmAndNltm|0|Enviar respostas LM e NTLM|
|lmNtlmAndNtlmV2|1|Enviar a segurança da sessão LM e o uso de NTLM NTLMv2 se negociado|
|lmAndNtlmOnly|2|Enviar respostas LM & NTLM somente|
|lmAndNtlmV2|3|Enviar respostas LM & NTLMv2 somente|
|lmNtlmV2AndNotLm|4|Envie respostas LM & NTLMv2 apenas. Recusar LM|
|lmNtlmV2AndNotLmOrNtm|5|Envie respostas LM & NTLMv2 apenas. Recusar LM & NTLM|





