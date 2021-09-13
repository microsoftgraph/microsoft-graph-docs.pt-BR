---
title: Tipo de número eapFastConfiguration
description: Configurações disponíveis para Configuração FAST EAP.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cd64a51bc9e41c1ea558ad4d1245b693de29f3c7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069184"
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



