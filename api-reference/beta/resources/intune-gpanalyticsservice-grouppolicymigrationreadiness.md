---
title: tipo de enumeração groupPolicyMigrationReadiness
description: Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e6b2ec4f8363f6ad68cd34a77287502eaadf2d52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524480"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>tipo de enumeração groupPolicyMigrationReadiness

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhuma|1 |Nenhuma cobertura do Intune|
|parcial|2 |Cobertura do Intune parcial|
|complete|3 |Cobertura completa do Intune|
|erro|4 |Erro ao analisar a cobertura|
|Não aplicável|5 |Nenhuma configuração de política de grupo no GPO|



