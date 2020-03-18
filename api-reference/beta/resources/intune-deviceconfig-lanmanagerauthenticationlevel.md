---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 670cb0bec6915b79102eae227a261f26eb052413
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790374"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>tipo de enumeração lanManagerAuthenticationLevel

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



