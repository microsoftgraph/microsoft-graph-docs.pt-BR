---
title: tipo de enum localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c39f2bb6d0bab2aff09fc05bb0492e81102e1b7c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396081"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>tipo de enum localSecurityOptionsMinimumSessionSecurity

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Enviar LM & respostas NTLM|
|requireNtmlV2SessionSecurity|1|Enviar a segurança da sessão do LM & usar NTLM NTLMv2 se negociado|
|require128BitEncryption|2|Enviar LM & somente respostas NTLM|
|ntlmV2And128BitEncryption|3|Enviar LM & respostas NTLMv2|




