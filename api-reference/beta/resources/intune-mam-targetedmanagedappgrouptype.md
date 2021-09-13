---
title: tipo de número targetedManagedAppGroupType
description: Indica uma coleção de aplicativos destinados que podem ser uma das várias listas pré-definidas de aplicativos ou uma lista de aplicativos selecionada manualmente
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1b6dc30701baa475db098a48fe4bfce92b1e940c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063878"
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



