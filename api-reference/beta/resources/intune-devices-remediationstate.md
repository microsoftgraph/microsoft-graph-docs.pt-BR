---
title: tipo de enumeração remediable
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cd940bbe2256baa7954e67ba9469ac00740f4ad1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783911"
---
# <a name="remediationstate-enum-type"></a>tipo de enumeração remediable

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de status de execução do script de gerenciamento de dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Resultado desconhecido.|
|ignorados|1|A execução do script de correção foi ignorada|
|sucesso|duas|O script de correção foi executado com êxito e corrigiu o estado do dispositivo|
|remediationFailed|3D|O script de correção foi executado com êxito, mas falhou ao corrigir o estado do dispositivo|
|scriptError|4 |Execução de script de correção encontrada e erro ou tempo limite esgotado|



