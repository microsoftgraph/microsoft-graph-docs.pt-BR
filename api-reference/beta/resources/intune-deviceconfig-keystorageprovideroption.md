---
title: tipo de enum keyStorageProviderOption
description: Opções de importação do armazenamento de chave KSP (provedor).
author: tfitzmac
ms.openlocfilehash: 7923dd5c4b8a09d834d29b65928430828f3dafac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342214"
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





