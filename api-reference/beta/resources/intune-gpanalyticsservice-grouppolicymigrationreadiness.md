---
title: tipo denum groupPolicyMigrationReadiness
description: Indica se o arquivo de Objeto de Política de Grupo está coberto e pronto para migração do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3e1b02c804268a4eadb0503f3bab53ff37c95563
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58782928"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>tipo denum groupPolicyMigrationReadiness

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica se o arquivo de Objeto de Política de Grupo está coberto e pronto para migração do Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|1|Sem cobertura do Intune|
|partial|2|Cobertura parcial do Intune|
|complete|3|Cobertura completa do Intune|
|erro|4 |Erro ao analisar a cobertura|
|notApplicable|5 |Sem configurações de Política de Grupo no GPO|



