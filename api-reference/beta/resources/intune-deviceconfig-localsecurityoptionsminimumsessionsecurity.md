---
title: tipo de enum localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 822c996d788fd5edb5c92f876c725b771b051c15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952479"
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





