---
title: tipo de enumeração remediable
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fb46c05ddbd1055f44794f0300077d47122aea25
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081115"
---
# <a name="remediationstate-enum-type"></a>tipo de enumeração remediable

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de status de execução do script de gerenciamento de dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Resultado desconhecido.|
|ignorados|1 |A execução do script de correção foi ignorada|
|sucesso|2 |O script de correção foi executado com êxito e corrigiu o estado do dispositivo|
|remediationFailed|3D|O script de correção foi executado com êxito, mas falhou ao corrigir o estado do dispositivo|
|scriptError|4 |Execução de script de correção encontrada e erro ou tempo limite esgotado|






