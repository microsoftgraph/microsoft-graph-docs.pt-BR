---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8580688edbdacb150a37ee5cf2a52fdc77dd490f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526252"
---
# <a name="keystorageprovideroption-enum-type"></a>tipo de enumeração keyStorageProviderOption

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Opções de importação do KSP (provedor de armazenamento de chave).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|,0|Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, importe para o KSP de software.|
|useTpmKspOtherwiseFail|1 |Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, falha.|
|usePassportForWorkKspOtherwiseFail|2 |Importe para o Passport para trabalho do KSP, se disponível, caso contrário, falha.|
|useSoftwareKsp|3 |Importar para KSP de software.|



