---
title: tipo denum groupPolicyOperationType
description: Tipo de operação de Política de Grupo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0b16ce7f8733aa5c0e3bfe03591fdf37b357fe0f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046838"
---
# <a name="grouppolicyoperationtype-enum-type"></a>tipo denum groupPolicyOperationType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de operação de Política de Grupo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|0|Tipo de operação inválido da Política de Grupo.|
|upload|1|Tipo de operação de carregamento da Política de Grupo.|
|uploadNewVersion|2|A Política de Grupo carrega o novo tipo de operação de versão.|
|addLanguageFiles|3|Política de Grupo adicionar novo tipo de operação de arquivos de idioma (ADML).|
|removeLanguageFiles|4 |Tipo de operação de arquivos ADML (remover idioma) da Política de Grupo.|
|updateLanguageFiles|5 |Tipo de operação de arquivos ADML (idioma de atualização de Política de Grupo).|
|remove|6 |Política de Grupo remova o tipo de operação de arquivo carregado.|



