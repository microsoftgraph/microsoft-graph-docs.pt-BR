---
title: tipo de enumeração macOSSoftwareUpdateState
description: Estado de atualização do software MacOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 05d2d951d8eacb93d952e20f01af6e42b30eecc1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731075"
---
# <a name="macossoftwareupdatestate-enum-type"></a>tipo de enumeração macOSSoftwareUpdateState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de atualização do software MacOS

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|sucesso|,0|A atualização de software foi instalada com êxito|
|Baixe|1000|A atualização de software está sendo baixada|
|terminado|1001|A atualização de software foi baixada|
|instalado|1002|A atualização de software está sendo instalada|
|Estado|1003|Nenhuma ação está sendo executada nesta atualização de software|
|disponível|1004|A atualização de software está disponível no dispositivo|
|agendado|1005|A atualização de software foi agendada no dispositivo|
|downloadFailed|2000|Falha no download da atualização de software|
|downloadInsufficientSpace|2001|Não há espaço suficiente para baixar a atualização|
|downloadInsufficientPower|2002|Não há energia suficiente para baixar a atualização|
|downloadInsufficientNetwork|2003|Não há capacidade de rede suficiente para baixar a atualização|
|installInsufficientSpace|2004|Não há espaço suficiente para instalar a atualização|
|installInsufficientPower|2005|Não há energia suficiente para instalar a atualização|
|installFailed|2006|A instalação falhou por um motivo não especificado|
|commandFailed|2007|O comando Schedule Update falhou por um motivo não especificado|





