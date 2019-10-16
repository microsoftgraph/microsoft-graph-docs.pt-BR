---
title: tipo de enumeração remediable
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b359842d7fb266803fdb758d32ca51e6a4b78b97
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529085"
---
# <a name="remediationstate-enum-type"></a>tipo de enumeração remediable

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de status de execução do script de gerenciamento de dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Resultado desconhecido.|
|ignorados|1|A execução do script de correção foi ignorada|
|sucesso|duas|O script de correção foi executado com êxito e corrigiu o estado do dispositivo|
|remediationFailed|3D|O script de correção foi executado com êxito, mas falhou ao corrigir o estado do dispositivo|
|scriptError|4 |Execução de script de correção encontrada e erro ou tempo limite esgotado|



