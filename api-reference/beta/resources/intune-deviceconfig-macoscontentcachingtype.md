---
title: tipo de enumeração macOSContentCachingType
description: Indica o tipo de conteúdo que pode ser armazenado em cache pelo serviço de cache de conteúdo da Apple.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: aed963885b7ef65ea5feaa8df443a6981343929b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790177"
---
# <a name="macoscontentcachingtype-enum-type"></a>tipo de enumeração macOSContentCachingType

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de conteúdo que pode ser armazenado em cache pelo serviço de cache de conteúdo da Apple.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|,0|Padrão. Os dados de iCloud do usuário e os dados não iCloud serão armazenados em cache.|
|userContentOnly|1 |Permitir que o serviço de cache de conteúdo da Apple armazene em cache os dados do iCloud.|
|sharedContentOnly|duas|Permitir que o serviço de cache de conteúdo da Apple armazene em cache dados não iCloud (por exemplo, atualizações de aplicativo e software).|



