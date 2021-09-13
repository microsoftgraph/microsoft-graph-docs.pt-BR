---
title: Tipo denum lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ff913766f41dfa3ec1a53c3a1ba37fc94cbc2b23
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127084"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>Tipo denum lanManagerAuthenticationLevel

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para LanManagerAuthenticationLevel

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|lmAndNltm|0|Enviar respostas & NTLM de LM|
|lmNtlmAndNtlmV2|1|Enviar a segurança de sessão NTLMv2 & lm se negociada|
|lmAndNtlmOnly|2|Enviar somente & NTLM|
|lmAndNtlmV2|3|Enviar somente & NTLMv2|
|lmNtlmV2AndNotLm|4 |Envie somente & NTLMv2. Recusar LM|
|lmNtlmV2AndNotLmOrNtm|5 |Envie somente & NTLMv2. Recusar LM & NTLM|



