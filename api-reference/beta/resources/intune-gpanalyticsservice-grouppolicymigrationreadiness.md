---
title: tipo denum groupPolicyMigrationReadiness
description: Indica se o arquivo de Objeto de Política de Grupo está coberto e pronto para migração do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4c965cf4a18f025c8f45e9ef46f5d5e26658dbbc9993c947c35f3fc6cdf7d77d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224555"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>tipo denum groupPolicyMigrationReadiness

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica se o arquivo de Objeto de Política de Grupo está coberto e pronto para migração do Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|1 |Sem cobertura do Intune|
|partial|2|Cobertura parcial do Intune|
|complete|3 |Cobertura completa do Intune|
|erro|4 |Erro ao analisar a cobertura|
|notApplicable|5 |Sem configurações de Política de Grupo no GPO|




