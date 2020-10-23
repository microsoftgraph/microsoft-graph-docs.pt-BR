---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b71f045ac937af455da428b98242f9d074b14840
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732534"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>tipo de enumeração lanManagerAuthenticationLevel

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para LanManagerAuthenticationLevel

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|lmAndNltm|,0|Enviar respostas LM & NTLM|
|lmNtlmAndNtlmV2|1|Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada|
|lmAndNtlmOnly|duas|Enviar somente respostas LM & NTLM|
|lmAndNtlmV2|3D|Enviar somente respostas LM & NTLMv2|
|lmNtlmV2AndNotLm|4 |Enviar LM & somente respostas NTLMv2. Recusar LM|
|lmNtlmV2AndNotLmOrNtm|5 |Enviar LM & somente respostas NTLMv2. Recusar LM & NTLM|





