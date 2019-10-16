---
title: tipo de enumeração groupPolicyMigrationReadiness
description: Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fb87c31bfe92a8845953e6e2a264ec60c9a3d863
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539103"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>tipo de enumeração groupPolicyMigrationReadiness

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|1|Nenhuma cobertura do Intune|
|parcial|duas|Cobertura do Intune parcial|
|complete|3D|Cobertura completa do Intune|
|erro|4 |Erro ao analisar a cobertura|
|Não aplicável|5 |Nenhuma configuração de política de grupo no GPO|



