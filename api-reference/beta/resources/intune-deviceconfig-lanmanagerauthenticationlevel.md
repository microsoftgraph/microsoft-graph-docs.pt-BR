---
title: Tipo denum lanManagerAuthenticationLevel
description: Valores possíveis para LanManagerAuthenticationLevel
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b38f720076d56605f31525dc4cb83a328ec977b37b064ffef7bb9d221444bcc6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54185856"
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
|lmNtlmAndNtlmV2|1 |Enviar a segurança de sessão NTLMv2 & lm se negociada|
|lmAndNtlmOnly|2|Enviar somente & NTLM|
|lmAndNtlmV2|3 |Enviar somente & NTLMv2|
|lmNtlmV2AndNotLm|4 |Envie somente & NTLMv2. Recusar LM|
|lmNtlmV2AndNotLmOrNtm|5 |Envie somente & NTLMv2. Recusar LM & NTLM|




