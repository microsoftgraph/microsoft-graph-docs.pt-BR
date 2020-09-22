---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1789debbbc672d0ee195af788292fd556d25e899
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029327"
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
|venceu|2 |O token expirou.|
|Inválido|3 |O token é inválido.|
|assignedToExternalMDM|4 |O token é gerenciado por outro serviço MDM.|
|duplicateLocationId|5 |O token é associado ao mesmo local de outro token na conta.|






