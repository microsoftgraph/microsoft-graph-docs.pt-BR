---
title: tipo de enumeração keyStorageProviderOption
description: Opções de importação do KSP (provedor de armazenamento de chave).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d0a0fca9dd77a4c83022d875350f12a3e56e18d6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301428"
---
# <a name="keystorageprovideroption-enum-type"></a>tipo de enumeração keyStorageProviderOption

Namespace: microsoft.graph

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




