---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ed06e011bbd9f64645541ded8929b0f2b5984fc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989424"
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





