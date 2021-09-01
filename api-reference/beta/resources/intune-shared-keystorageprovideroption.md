---
title: Tipo de número keyStorageProviderOption
description: Opções de importação Armazenamento KSP (Provedor de Chaves).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e6dc213f3cef76380a5bf40d91b6220e1408783f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786274"
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



