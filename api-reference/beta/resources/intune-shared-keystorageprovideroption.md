---
title: Tipo de número keyStorageProviderOption
description: Opções de importação Armazenamento KSP (Provedor de Chaves).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7bfd89c8e74264aca79af72325d6b5b4a96b23a3a3fadd44b32c94f3fa95cc58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54219749"
---
# <a name="keystorageprovideroption-enum-type"></a>Tipo de número keyStorageProviderOption

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Opções de importação Armazenamento KSP (Provedor de Chaves).

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|Importar para KSP de Módulo de Plataforma Confiável (TPM) se presente, caso contrário, importe para o KSP de software.|
|useTpmKspOtherwiseFail|1 |Importar para KSP de Módulo de Plataforma Confiável (TPM) se presente, caso contrário, falhará.|
|usePassportForWorkKspOtherwiseFail|2|Importar para Passport para KSP de trabalho, se disponível, caso contrário, falhará.|
|useSoftwareKsp|3 |Importar para KSP de software.|




