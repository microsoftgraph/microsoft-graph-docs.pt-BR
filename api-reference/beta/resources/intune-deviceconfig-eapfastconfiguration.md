---
title: Tipo de número eapFastConfiguration
description: Configurações disponíveis para Configuração FAST EAP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 880d5b3456f07d8df495b56adece254aa8e5e317
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795232"
---
# <a name="eapfastconfiguration-enum-type"></a>Tipo de número eapFastConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configurações disponíveis para Configuração FAST EAP.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|noProtectedAccessCredential|0|Use o EAP-FAST sem a Credencial de Acesso Protegido (PAC).|
|useProtectedAccessCredential|1|Use a Credencial de Acesso Protegido (PAC).|
|useProtectedAccessCredentialAndProvision|2|Use o PAC (Credencial de Acesso Protegido) e o PAC de provisionamento.|
|useProtectedAccessCredentialAndProvisionAnonymously|3|Use a Credencial de Acesso Protegido (PAC), Provisione PAC e faça isso anonimamente.|



