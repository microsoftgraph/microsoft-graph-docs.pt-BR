---
title: Tipo denum safeSearchFilterType
description: Especifica que nível de pesquisa segura (filtragem de conteúdo adulto) é necessário
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: adf5460c702b5779591152d5241cf66f22af0e6f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091619"
---
# <a name="safesearchfiltertype-enum-type"></a>Tipo denum safeSearchFilterType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Especifica que nível de pesquisa segura (filtragem de conteúdo adulto) é necessário

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|User Defined, default value, no intent.|
|strict|1|Filtragem estrita e mais alta em relação ao conteúdo adulto.|
|moderada|2|Filtragem moderada em relação ao conteúdo adulto (os resultados válidos da pesquisa não serão filtrados).|



