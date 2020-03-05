---
title: tipo de enumeração edgeKioskModeRestrictionType
description: Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 929e74097d329f2d6932ae3aadaa001258dbd2fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530057"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a>tipo de enumeração edgeKioskModeRestrictionType

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Especifique como as configurações do Microsoft Edge são restritas com base no modo quiosque.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Não configurado (Irrestrito).|
|digitalSignage|1 |Pôsteres/digitais no modo de aplicativo único.|
|normalmode|2 |Modo normal (versão completa do Microsoft Edge).|
|publicBrowsingSingleApp|3 |Navegação pública no modo de aplicativo único.|
|publicBrowsingMultiApp|4 |Navegação pública (InPrivate) no modo de vários aplicativos.|



