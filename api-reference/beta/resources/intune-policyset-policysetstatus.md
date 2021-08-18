---
title: Tipo de número policySetStatus
description: O número para especificar o status de PolicySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a31849f4984edbabdda45e319df9a8cba5005cb76302f8b68dc414ef7a59b651
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54150182"
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
|validação|1 |Todos os itens PolicySet agora estão validando para configurações correspondentes de cargas de trabalho.|
|partialSuccess|2|Pós-processo concluído para todos os itens PolicySet, mas há falhas.|
|sucesso|3 |Todos os itens PolicySet são implantados. Não significa que toda a implantação foi bem-sucedida. |
|erro|4 |O processamento policySet falhou completamente.|
|notAssigned|5 |PolicySet/PolicySetItem não é atribuído a nenhum grupo.|




