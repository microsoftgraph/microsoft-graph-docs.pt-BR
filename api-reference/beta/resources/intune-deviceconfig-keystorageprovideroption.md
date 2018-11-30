---
title: tipo de enum keyStorageProviderOption
description: Opções de importação do armazenamento de chave KSP (provedor).
ms.openlocfilehash: 236489d288ec0be70a818e1c51b8c634ad3933a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034040"
---
# <a name="keystorageprovideroption-enum-type"></a>tipo de enum keyStorageProviderOption

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Opções de importação do armazenamento de chave KSP (provedor).
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário, importe para KSP de Software.|
|useTpmKspOtherwiseFail|1|Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário falhar.|
|usePassportForWorkKspOtherwiseFail|2|Importar Passport trabalho KSP se estiver disponível, caso contrário falhar.|
|useSoftwareKsp|3|Importação ao Software KSP.|





