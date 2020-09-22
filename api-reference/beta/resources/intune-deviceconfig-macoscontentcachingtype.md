---
title: tipo de enumeração macOSContentCachingType
description: Indica o tipo de conteúdo que pode ser armazenado em cache pelo serviço de cache de conteúdo da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9022b320507cc10455e2eeb3ebd3a3ca58d52f71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993837"
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
|sharedContentOnly|2 |Permitir que o serviço de cache de conteúdo da Apple armazene em cache dados não iCloud (por exemplo, atualizações de aplicativo e software).|






