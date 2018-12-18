---
title: tipo de enum lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: tfitzmac
ms.openlocfilehash: fd5d63f262b9b6e9a27060725e721cb81c495a57
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308740"
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





