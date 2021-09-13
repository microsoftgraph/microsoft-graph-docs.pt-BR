---
title: tipo de número localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d3ecff15416ff3d313840d7b3a0ca33c2ef83e3b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033683"
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
|requireNtmlV2SessionSecurity|1|Enviar a segurança de sessão NTLMv2 & lm se negociada|
|require128BitEncryption|2|Enviar somente & NTLM|
|ntlmV2And128BitEncryption|3|Enviar somente & NTLMv2|



