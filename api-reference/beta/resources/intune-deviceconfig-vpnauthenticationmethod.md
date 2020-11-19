---
title: tipo de enumeração vpnAuthenticationMethod
description: Método de autenticação VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3ffc71fa17385ad1e0d00dd77958e65fb7a4aed9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276312"
---
# <a name="vpnauthenticationmethod-enum-type"></a>tipo de enumeração vpnAuthenticationMethod

Namespace: microsoft.graph

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
|azureAD|4 |Usar o Azure AD para autenticação.|




