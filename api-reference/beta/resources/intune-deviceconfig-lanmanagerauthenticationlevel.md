---
title: tipo de enum lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fd88deb7684301023a75905d12a59ce25bad750f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911991"
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





