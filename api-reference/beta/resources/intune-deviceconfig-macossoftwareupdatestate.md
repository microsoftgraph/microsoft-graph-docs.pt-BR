---
title: Tipo de número macOSSoftwareUpdateState
description: Estado de Atualização de Software MacOS
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3459390263c0494a9c67e83a9f1cb4579db283e2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054489"
---
# <a name="macossoftwareupdatestate-enum-type"></a>Tipo de número macOSSoftwareUpdateState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de Atualização de Software MacOS

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|sucesso|0|A atualização de software instalada com êxito|
|download|1000|A atualização de software está sendo baixada|
|baixado|1001|A atualização de software foi baixada|
|instalando|1002|A atualização de software está sendo instalada|
|idle|1003|Nenhuma ação está sendo tomada nesta atualização de software|
|disponível|1004|A atualização de software está disponível no dispositivo|
|agendado|1005|A atualização de software foi agendada no dispositivo|
|downloadFailed|2000|O download de atualização de software falhou|
|downloadInsufficientSpace|2001|Não há espaço suficiente para baixar a atualização|
|downloadInsufficientPower|2002|Não há energia suficiente para baixar a atualização|
|downloadInsufficientNetwork|2003|Não há capacidade de rede insuficiente para baixar a atualização|
|installInsufficientSpace|2004|Não há espaço suficiente para instalar a atualização|
|installInsufficientPower|2005|Não há energia suficiente para instalar a atualização|
|installFailed|2006|A instalação falhou por um motivo não especificado|
|commandFailed|2007|O comando de atualização de agendamento falhou por um motivo não especificado|



