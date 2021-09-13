---
title: tipo denum groupPolicyMigrationReadiness
description: Indica se o arquivo de Objeto de Política de Grupo está coberto e pronto para migração do Intune.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1b65c8f739e4c93d8881e12b8b715e4bfc7aa7ef
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057303"
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



