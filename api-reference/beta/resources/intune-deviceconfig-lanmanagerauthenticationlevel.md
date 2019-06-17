---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a80aefec83c0c2a577af9b8dfed5dcea1ff7d79
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989347"
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
|lmNtlmV2AndNotLm|quatro|Enviar LM & somente respostas NTLMv2. Recusar LM|
|lmNtlmV2AndNotLmOrNtm|0,5|Enviar LM & somente respostas NTLMv2. Recusar LM & NTLM|





