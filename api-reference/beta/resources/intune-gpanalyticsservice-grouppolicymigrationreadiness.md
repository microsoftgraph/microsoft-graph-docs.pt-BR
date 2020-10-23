---
title: tipo de enumeração groupPolicyMigrationReadiness
description: Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d860844de50c58deace7f10821ca0b1a4591d00b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722820"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>tipo de enumeração groupPolicyMigrationReadiness

Namespace: microsoft.graph

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





