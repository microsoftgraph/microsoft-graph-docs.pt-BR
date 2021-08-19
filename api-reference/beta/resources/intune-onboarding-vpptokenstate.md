---
title: Tipo denum vppTokenState
description: Estados possíveis associados a um token do Programa de Compra de Volume da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f7df4f078b91a6c42ac4718a30145e1e141d8436bd8932c25780ce678cf2366c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54172782"
---
# <a name="vpptokenstate-enum-type"></a>Tipo denum vppTokenState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estados possíveis associados a um token do Programa de Compra de Volume da Apple.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Estado padrão.|
|valid|1 |Token é válido.|
|expirado|2|O token expirou.|
|Inválido|3 |Token é inválido.|
|assignedToExternalMDM|4 |Token é gerenciado por outro Serviço MDM.|
|duplicateLocationId|5 |Token é associado ao mesmo local que outro token na conta.|




