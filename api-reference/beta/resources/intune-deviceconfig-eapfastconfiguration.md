---
title: tipo de enum eapFastConfiguration
description: Configurações disponíveis para a configuração de EAP-FAST.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65165929d388ed57f2651a0d277996e56d2f046e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954453"
---
# <a name="eapfastconfiguration-enum-type"></a>tipo de enum eapFastConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configurações disponíveis para a configuração de EAP-FAST.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|noProtectedAccessCredential|0|Use EAP-FAST sem credencial de acesso protegido (PAC).|
|useProtectedAccessCredential|1|Uso protegido credencial de acesso (PAC).|
|useProtectedAccessCredentialAndProvision|2|Uso Protected Access credencial (PAC) e provisionar PAC.|
|useProtectedAccessCredentialAndProvisionAnonymously|3|Use credenciais PAC (Protected Access), provisão PAC e fazê-lo anonimamente.|





