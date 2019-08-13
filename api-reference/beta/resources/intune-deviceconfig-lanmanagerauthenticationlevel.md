---
title: tipo de enumeração lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ade139765c9a362cd0c9f9365af0026c51ecb4ce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356722"
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



