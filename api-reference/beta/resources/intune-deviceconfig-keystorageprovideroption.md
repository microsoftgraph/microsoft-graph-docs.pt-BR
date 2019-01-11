---
title: tipo de enum keyStorageProviderOption
description: Opções de importação do armazenamento de chave KSP (provedor).
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4609092c3022b62331bbb6226a5b91e4b287ff79
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826464"
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





