---
title: Tipo denum macOSContentCachingType
description: Indica o tipo de conteúdo permitido para ser armazenado em cache pelo serviço de cache de conteúdo da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0bb0859eb7b409849341b03f51abb838c62f2a18
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783537"
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
|userContentOnly|1|Permitir que o serviço de cache de conteúdo da Apple cache de dados do iCloud do usuário.|
|sharedContentOnly|2|Permitir que o serviço de cache de conteúdo da Apple cache de dados que não são do iCloud (por exemplo, atualizações de aplicativo e software).|



