---
title: tipo de enumeração groupPolicyMigrationReadiness
description: Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 30d223eb59d092b9411388b93226d48165a4e703
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298761"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>tipo de enumeração groupPolicyMigrationReadiness

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica se o arquivo de objeto de diretiva de grupo está coberto e pronto para a migração do Intune.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|nenhum|1|Nenhuma cobertura do Intune|
|parcial|duas|Cobertura do Intune parcial|
|complete|3D|Cobertura completa do Intune|
|erro|4 |Erro ao analisar a cobertura|
|Não aplicável|5 |Nenhuma configuração de política de grupo no GPO|




