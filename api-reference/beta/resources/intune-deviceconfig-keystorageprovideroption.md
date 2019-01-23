---
title: tipo de enum keyStorageProviderOption
description: Opções de importação do armazenamento de chave KSP (provedor).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6993d7e241ef94c572975c709c286a14f6eabf5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424221"
---
# <a name="keystorageprovideroption-enum-type"></a>tipo de enum keyStorageProviderOption

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Opções de importação do armazenamento de chave KSP (provedor).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário, importe para KSP de Software.|
|useTpmKspOtherwiseFail|1|Importação para Trusted Platform Module (TPM) KSP se presente, caso contrário falhar.|
|usePassportForWorkKspOtherwiseFail|2|Importar Passport trabalho KSP se estiver disponível, caso contrário falhar.|
|useSoftwareKsp|3|Importação ao Software KSP.|




