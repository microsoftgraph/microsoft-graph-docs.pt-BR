---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a087c9d99164ce5c830b2d40022d7ddd99736547
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806395"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>tipo de enumeração localSecurityOptionsMinimumSessionSecurity

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhuma|,0|Enviar respostas LM & NTLM|
|requireNtmlV2SessionSecurity|1|Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada|
|require128BitEncryption|duas|Enviar somente respostas LM & NTLM|
|ntlmV2And128BitEncryption|3D|Enviar somente respostas LM & NTLMv2|





