---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 182c375ae8e70e7190f9860a72d04e7f508bc61e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001030"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>tipo de enumeração localSecurityOptionsMinimumSessionSecurity

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|,0|Enviar respostas LM & NTLM|
|requireNtmlV2SessionSecurity|1|Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada|
|require128BitEncryption|duas|Enviar somente respostas LM & NTLM|
|ntlmV2And128BitEncryption|3D|Enviar somente respostas LM & NTLMv2|





