---
title: Tipo de número vpnAuthenticationMethod
description: Método de autenticação VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0fca9d52b09bdb19f85aa6fa06c166195263af39fbf143e956207f7a5e0a7b30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226340"
---
# <a name="vpnauthenticationmethod-enum-type"></a>Tipo de número vpnAuthenticationMethod

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Método de autenticação VPN.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|certificado|0|Autenticar com um certificado.|
|usernameAndPassword|1 |Use nome de usuário e senha para autenticação.|
|sharedSecret|2|Use o Segredo Compartilhado para Autenticação.  Válido somente para iOS IKEv2.|
|derivedCredential|3 |Use a Credencial Derivada para Autenticação.|
|azureAD|4 |Use o Azure AD para autenticação.|




