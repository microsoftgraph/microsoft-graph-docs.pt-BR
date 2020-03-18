---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a2612aeb2cded950023a14136b71a8c7a55555a9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790409"
---
# <a name="keystorageprovideroption-enum-type"></a>tipo de enumeração keyStorageProviderOption

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Opções de importação do KSP (provedor de armazenamento de chave).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|,0|Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, importe para o KSP de software.|
|useTpmKspOtherwiseFail|1|Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, falha.|
|usePassportForWorkKspOtherwiseFail|duas|Importe para o Passport para trabalho do KSP, se disponível, caso contrário, falha.|
|useSoftwareKsp|3D|Importar para KSP de software.|



