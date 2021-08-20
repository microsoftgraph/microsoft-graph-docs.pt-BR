---
title: tipo de número localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b16a4a3e1e98612af7a69b63a02fcdd681d4fa7842134681603b54abcf33e648
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54136307"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>tipo de número localSecurityOptionsMinimumSessionSecurity

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Enviar respostas & NTLM de LM|
|requireNtmlV2SessionSecurity|1 |Enviar a segurança de sessão NTLMv2 & lm se negociada|
|require128BitEncryption|2|Enviar somente & NTLM|
|ntlmV2And128BitEncryption|3 |Enviar somente & NTLMv2|




