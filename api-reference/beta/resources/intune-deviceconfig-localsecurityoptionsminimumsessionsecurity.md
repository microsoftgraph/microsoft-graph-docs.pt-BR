---
title: tipo de enum localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
ms.openlocfilehash: 969c7d6576c613f5214bfc3b8a5a1ad36722f0df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038996"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>tipo de enum localSecurityOptionsMinimumSessionSecurity

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhum|0|Enviar respostas LM e NTLM|
|requireNtmlV2SessionSecurity|1|Enviar a segurança da sessão LM e o uso de NTLM NTLMv2 se negociado|
|require128BitEncryption|2|Enviar respostas LM & NTLM somente|
|ntlmV2And128BitEncryption|3|Enviar respostas LM & NTLMv2 somente|





