---
title: tipo de enumeração policySetStatus
description: A enumeração para especificar o status de Policyset.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a41e4f3dc01bd04c915dc4c883bae640b3e7683
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199631"
---
# <a name="policysetstatus-enum-type"></a>tipo de enumeração policySetStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A enumeração para especificar o status de Policyset.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Valor padrão.|
|conclui|1|Todos os itens de Policyset agora estão sendo validados para as configurações correspondentes de cargas de trabalho.|
|partialSuccess|duas|Processo de post concluído para todos os itens de Policyset, mas há falhas.|
|sucesso|3D|Todos os itens de Policyset são implantados. Não significa que toda a implantação tenha sido bem-sucedida. |
|erro|quatro|Falha total no processamento de policyset.|
|Não atribuído|0,5|Policyset/PolicySetItem não é atribuído a nenhum grupo.|



