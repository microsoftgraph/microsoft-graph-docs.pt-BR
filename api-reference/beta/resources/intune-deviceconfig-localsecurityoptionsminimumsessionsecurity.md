---
title: tipo de enum localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fb6912e7d3bba42364849165cceb28050ddacfae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833233"
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





