---
title: tipo de enumeração policySetStatus
description: A enumeração para especificar o status de Policyset.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a470e6c13bfd20ada920bbe2b471bfa96379092
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775146"
---
# <a name="policysetstatus-enum-type"></a>tipo de enumeração policySetStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A enumeração para especificar o status de Policyset.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Valor padrão.|
|conclui|1|Todos os itens de Policyset agora estão sendo validados para as configurações correspondentes de cargas de trabalho.|
|partialSuccess|duas|Processo de post concluído para todos os itens de Policyset, mas há falhas.|
|sucesso|3D|Todos os itens de Policyset são implantados. Não significa que toda a implantação tenha sido bem-sucedida. |
|erro|4 |Falha total no processamento de policyset.|
|Não atribuído|5 |Policyset/PolicySetItem não é atribuído a nenhum grupo.|



