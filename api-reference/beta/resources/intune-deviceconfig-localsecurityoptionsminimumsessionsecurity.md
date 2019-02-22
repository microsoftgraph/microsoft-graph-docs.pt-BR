---
title: tipo de enumeração localSecurityOptionsMinimumSessionSecurity
description: Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe6007747aed1037a4dc3d5264bb432182a28c00
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145343"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>tipo de enumeração localSecurityOptionsMinimumSessionSecurity

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para LocalSecurityOptionsMinimumSessionSecurity

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|,0|Enviar respostas LM & NTLM|
|requireNtmlV2SessionSecurity|1|Send LM & NTLM-use a segurança da sessão NTLMv2, se estiver negociada|
|require128BitEncryption|duas|Enviar somente respostas LM & NTLM|
|ntlmV2And128BitEncryption|3D|Enviar somente respostas LM & NTLMv2|




