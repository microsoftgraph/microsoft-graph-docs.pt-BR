---
title: tipo de enumeração appListType
description: Valores possíveis da lista de aplicativos de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 379ec2e10e68d62353875cd2b49c0944fe11f4da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575097"
---
# <a name="applisttype-enum-type"></a>tipo de enumeração appListType

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis da lista de aplicativos de conformidade.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Nenhuma|,0|Valor padrão, sem intenção.|
|appsInListCompliant|1 |A lista representa os aplicativos que serão considerados compatíveis (apenas os aplicativos na lista são compatíveis).|
|appsNotInListCompliant|2 |A lista representa os aplicativos que serão considerados não compatíveis (todos os aplicativos são compatíveis, exceto os aplicativos na lista).|



