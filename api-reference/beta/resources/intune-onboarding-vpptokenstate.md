---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8a159a5a2e359cef6978df44a8f40a1d664dfa48
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259400"
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
|inválido|1|O token é válido.|
|venceu|duas|O token expirou.|
|Inválido|3D|O token é inválido.|
|assignedToExternalMDM|4 |O token é gerenciado por outro serviço MDM.|
|duplicateLocationId|5 |O token é associado ao mesmo local de outro token na conta.|




