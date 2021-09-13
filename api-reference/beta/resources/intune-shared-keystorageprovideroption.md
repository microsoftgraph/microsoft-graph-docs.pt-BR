---
title: Tipo de número keyStorageProviderOption
description: Opções de importação Armazenamento KSP (Provedor de Chaves).
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9f8f47384333189f80d6443a17027e62b1a1e465
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030001"
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
|useTpmKspOtherwiseFail|1|Importar para KSP de Módulo de Plataforma Confiável (TPM) se presente, caso contrário, falhará.|
|usePassportForWorkKspOtherwiseFail|2|Importar para Passport para KSP de trabalho, se disponível, caso contrário, falhará.|
|useSoftwareKsp|3|Importar para KSP de software.|



