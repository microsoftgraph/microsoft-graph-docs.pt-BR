---
title: Tipo denum macOSContentCachingType
description: Indica o tipo de conteúdo permitido para ser armazenado em cache pelo serviço de cache de conteúdo da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d97afd473185a7a25959049322a5946012d5ad207a67c0ae4e1b7c659f59534c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206596"
---
# <a name="macoscontentcachingtype-enum-type"></a>Tipo denum macOSContentCachingType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de conteúdo permitido para ser armazenado em cache pelo serviço de cache de conteúdo da Apple.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Padrão. Os dados do iCloud do usuário e os dados que não são do iCloud serão armazenados em cache.|
|userContentOnly|1 |Permitir que o serviço de cache de conteúdo da Apple cache de dados do iCloud do usuário.|
|sharedContentOnly|2|Permitir que o serviço de cache de conteúdo da Apple cache de dados que não são do iCloud (por exemplo, atualizações de aplicativo e software).|




