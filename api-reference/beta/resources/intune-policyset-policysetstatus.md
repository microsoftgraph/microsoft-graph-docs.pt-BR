---
title: Tipo de número policySetStatus
description: O número para especificar o status de PolicySet.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22091444272c3e88648e1e14483ec58ce6f78873
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020319"
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



