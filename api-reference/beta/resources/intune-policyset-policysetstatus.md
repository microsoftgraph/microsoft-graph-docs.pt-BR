---
title: Tipo de número policySetStatus
description: O número para especificar o status de PolicySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 384eb054757e2a71ff15b4af45d91cc940416adb
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58757899"
---
# <a name="policysetstatus-enum-type"></a>Tipo de número policySetStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O número para especificar o status de PolicySet.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Valor padrão.|
|validação|1|Todos os itens PolicySet agora estão validando para configurações correspondentes de cargas de trabalho.|
|partialSuccess|2|Pós-processo concluído para todos os itens PolicySet, mas há falhas.|
|sucesso|3|Todos os itens PolicySet são implantados. Não significa que toda a implantação foi bem-sucedida. |
|erro|4 |O processamento policySet falhou completamente.|
|notAssigned|5 |PolicySet/PolicySetItem não é atribuído a nenhum grupo.|



