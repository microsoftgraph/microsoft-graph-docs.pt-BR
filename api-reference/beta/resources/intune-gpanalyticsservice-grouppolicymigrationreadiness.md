---
title: tipo de enumeração groupPolicyMigrationReadiness
description: Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: efd579adb3c3408eda9b87ffb7f48e98c836065f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783169"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>tipo de enumeração groupPolicyMigrationReadiness

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|1|Nenhuma cobertura do Intune|
|parcial|duas|Cobertura do Intune parcial|
|complete|3D|Cobertura completa do Intune|
|erro|4 |Erro ao analisar a cobertura|
|Não aplicável|5 |Nenhuma configuração de política de grupo no GPO|



