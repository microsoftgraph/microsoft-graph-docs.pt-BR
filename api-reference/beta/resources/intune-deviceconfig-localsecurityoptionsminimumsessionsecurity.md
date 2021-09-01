---
title: tipo de número localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1ea1d1a0b1cb268bfa86838ec6afcb4f6751f634
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819147"
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



