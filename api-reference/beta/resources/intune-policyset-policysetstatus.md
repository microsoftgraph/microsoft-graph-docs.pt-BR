---
title: tipo de enumeração policySetStatus
description: A enumeração para especificar o status de Policyset.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 32ea9586ffee2ef112c58a1f88bdbdaefd654a04
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735154"
---
# <a name="policysetstatus-enum-type"></a>tipo de enumeração policySetStatus

Namespace: microsoft.graph

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





