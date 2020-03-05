---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4750d5bc4da34f1e627d2b324827f78f830bb219
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526217"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>tipo de enumeração localSecurityOptionsMinimumSessionSecurity

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhuma|,0|Enviar respostas LM & NTLM|
|requireNtmlV2SessionSecurity|1 |Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada|
|require128BitEncryption|2 |Enviar somente respostas LM & NTLM|
|ntlmV2And128BitEncryption|3 |Enviar somente respostas LM & NTLMv2|



