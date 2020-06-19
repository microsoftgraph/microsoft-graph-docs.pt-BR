---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c286785522405946776907a296e475924ba8d4a8
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793630"
---
# <a name="vpptokenstate-enum-type"></a>tipo de enumeração vppTokenState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estados possíveis associados a um token do Apple Volume Purchase Program.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Estado padrão.|
|inválido|1 |O token é válido.|
|venceu|duas|O token expirou.|
|Inválido|3D|O token é inválido.|
|assignedToExternalMDM|4 |O token é gerenciado por outro serviço MDM.|
|duplicateLocationId|5 |O token é associado ao mesmo local de outro token na conta.|



