---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e00c78f571d7425d1e957b8df22d0a1fbfa80f11
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033710"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>tipo de enumeração localSecurityOptionsMinimumSessionSecurity

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|,0|Enviar respostas LM & NTLM|
|requireNtmlV2SessionSecurity|1 |Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada|
|require128BitEncryption|2 |Enviar somente respostas LM & NTLM|
|ntlmV2And128BitEncryption|3 |Enviar somente respostas LM & NTLMv2|






