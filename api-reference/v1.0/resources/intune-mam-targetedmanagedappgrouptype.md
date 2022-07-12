---
title: Tipo de enumeração targetedManagedAppGroupType
description: Indica uma coleção de aplicativos a serem direcionados, que pode ser uma das várias listas pré-definidas de aplicativos ou uma lista de aplicativos selecionada manualmente
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e7c6dd39ff11f961f93d844a1b85f38f634ee343
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730585"
---
# <a name="targetedmanagedappgrouptype-enum-type"></a>Tipo de enumeração targetedManagedAppGroupType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica uma coleção de aplicativos a serem direcionados, que pode ser uma das várias listas pré-definidas de aplicativos ou uma lista de aplicativos selecionada manualmente

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|selectedPublicApps|0|Direcionou a coleção de aplicativos selecionados manualmente pelo administrador.|
|allCoreMicrosoftApps|1|Direcionar o conjunto principal de aplicativos da Microsoft (Office, Edge etc.).|
|allMicrosoftApps|2|Direcionar todos os aplicativos com a Microsoft como editor.|
|allApps|4|Direcionar todos os aplicativos com uma atribuição disponível.|





