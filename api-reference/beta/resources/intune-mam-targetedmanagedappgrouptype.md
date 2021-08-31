---
title: tipo de número targetedManagedAppGroupType
description: Indica uma coleção de aplicativos destinados que podem ser uma das várias listas pré-definidas de aplicativos ou uma lista de aplicativos selecionada manualmente
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 716a9e646c6e0b320869998d30f2995c65d60636
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817317"
---
# <a name="targetedmanagedappgrouptype-enum-type"></a>tipo de número targetedManagedAppGroupType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica uma coleção de aplicativos destinados que podem ser uma das várias listas pré-definidas de aplicativos ou uma lista de aplicativos selecionada manualmente

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|selectedPublicApps|0|Destino da coleção de aplicativos selecionados manualmente pelo administrador.|
|allCoreMicrosoftApps|1|Direcionar o conjunto principal de aplicativos da Microsoft (Office, Borda, etc.|
|allMicrosoftApps|2|Direcionar todos os aplicativos com a Microsoft como editor.|
|allApps|4 |Direcionar todos os aplicativos com uma atribuição disponível.|



