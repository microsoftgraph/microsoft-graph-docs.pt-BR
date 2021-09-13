---
title: Tipo de número windowsUpdateType
description: De quais dispositivos de filial receberão suas atualizações
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 03e5515adaa5e92aa90c5344d0891cff124be3cd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095413"
---
# <a name="windowsupdatetype-enum-type"></a>Tipo de número windowsUpdateType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

De quais dispositivos de filial receberão suas atualizações

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Permitir que o usuário desem conjunto.|
|all|1|Canal Semes anual (Direcionado). O dispositivo obtém todas as atualizações de recursos aplicáveis do Canal Semes anual (Direcionado).|
|businessReadyOnly|2|Canal Semes anual. O dispositivo obtém atualizações de recursos do Canal Semesanuais.|
|windowsInsiderBuildFast|3|Windows Insider build - Fast|
|windowsInsiderBuildSlow|4 |Windows Insider build - Slow|
|windowsInsiderBuildRelease|5 |Versão Windows build do Insider|



