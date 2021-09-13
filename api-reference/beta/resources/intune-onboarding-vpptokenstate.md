---
title: Tipo denum vppTokenState
description: Estados possíveis associados a um token do Programa de Compra de Volume da Apple.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a72b2be5a0ce4ff690e05c863cc7faad7023d0e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101160"
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
|valid|1|Token é válido.|
|expirado|2|O token expirou.|
|Inválido|3|Token é inválido.|
|assignedToExternalMDM|4 |Token é gerenciado por outro Serviço MDM.|
|duplicateLocationId|5 |Token é associado ao mesmo local que outro token na conta.|



