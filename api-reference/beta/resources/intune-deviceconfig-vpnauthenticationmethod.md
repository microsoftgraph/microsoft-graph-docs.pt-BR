---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 048b31bd835c1e94d3afcef87b6bd8e93f3ddeec
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787415"
---
# <a name="vpnauthenticationmethod-enum-type"></a>tipo de enumeração vpnAuthenticationMethod

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Método de autenticação VPN.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|certificado|,0|Autenticar com um certificado.|
|usernameAndPassword|1|Usar nome de usuário e senha para autenticação.|
|sharedSecret|duas|Usar segredo compartilhado para autenticação.  Válido somente para iOS IKEv2.|
|derivedCredential|3D|Use a credencial derivada para autenticação.|



