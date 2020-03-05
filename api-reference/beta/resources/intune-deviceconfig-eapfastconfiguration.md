---
title: tipo de enumeração eapFastConfiguration
description: Configurações disponíveis para a configuração EAP-FAST.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: db3f39eaeb375705c974e907ae4b0a177bd6c4ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526543"
---
# <a name="eapfastconfiguration-enum-type"></a>tipo de enumeração eapFastConfiguration

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configurações disponíveis para a configuração EAP-FAST.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|noProtectedAccessCredential|,0|Use EAP-FAST sem PAC (credencial de acesso protegido).|
|useProtectedAccessCredential|1 |Use a PAC (credencial de acesso protegido).|
|useProtectedAccessCredentialAndProvision|2 |Use a PAC (credencial de acesso protegido) e provisionar PAC.|
|useProtectedAccessCredentialAndProvisionAnonymously|3 |Use a PAC (credencial de acesso protegido), provisione PAC e faça isso de forma anônima.|



