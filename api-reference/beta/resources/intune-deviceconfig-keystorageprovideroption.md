---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b422443abcdb72cd76399ae9f2e0fea59bb6f34f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460419"
---
# <a name="keystorageprovideroption-enum-type"></a>tipo de enumeração keyStorageProviderOption

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Opções de importação do KSP (provedor de armazenamento de chave).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|,0|Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, importe para o KSP de software.|
|useTpmKspOtherwiseFail|1|Importar para KSP de Trusted Platform Module (TPM) se presente, caso contrário, falha.|
|usePassportForWorkKspOtherwiseFail|duas|Importe para o Passport para trabalho do KSP, se disponível, caso contrário, falha.|
|useSoftwareKsp|3D|Importar para KSP de software.|





