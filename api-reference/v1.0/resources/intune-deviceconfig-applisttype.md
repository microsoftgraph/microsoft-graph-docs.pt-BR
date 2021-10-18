---
title: Tipo de número appListType
description: Valores possíveis da lista de aplicativos de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a5410919bb33a4a77d4d774108157519fad9ae4d
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455918"
---
# <a name="applisttype-enum-type"></a>Tipo de número appListType

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis da lista de aplicativos de conformidade.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Valor padrão, sem intenção.|
|appsInListCompliant|1|A lista representa os aplicativos que serão considerados compatíveis (somente os aplicativos na lista são compatíveis).|
|appsNotInListCompliant|2|A lista representa os aplicativos que serão considerados não compatíveis (todos os aplicativos são compatíveis, exceto aplicativos na lista).|



