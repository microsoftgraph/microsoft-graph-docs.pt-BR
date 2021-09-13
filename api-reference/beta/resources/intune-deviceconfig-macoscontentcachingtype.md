---
title: Tipo denum macOSContentCachingType
description: Indica o tipo de conteúdo permitido para ser armazenado em cache pelo serviço de cache de conteúdo da Apple.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c61a195e2b0c3025ca3659bdcfacc4075fe9367d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017475"
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



