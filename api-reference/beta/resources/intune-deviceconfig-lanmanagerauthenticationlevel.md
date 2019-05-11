---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92cb5b32d8b4768af63d92461597c32f858c0a7c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946151"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>tipo de enumeração lanManagerAuthenticationLevel

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para LanManagerAuthenticationLevel

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|lmAndNltm|,0|Enviar respostas LM & NTLM|
|lmNtlmAndNtlmV2|1|Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada|
|lmAndNtlmOnly|duas|Enviar somente respostas LM & NTLM|
|lmAndNtlmV2|3D|Enviar somente respostas LM & NTLMv2|
|lmNtlmV2AndNotLm|quatro|Enviar somente respostas LM & NTLMv2. Recusar LM|
|lmNtlmV2AndNotLmOrNtm|0,5|Enviar somente respostas LM & NTLMv2. Recusar LM & NTLM|




