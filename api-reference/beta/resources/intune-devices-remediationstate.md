---
title: tipo de enumeração remediable
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dc2be0c860ba142f59bba05a2a0c5ae0105c0ab1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528511"
---
# <a name="remediationstate-enum-type"></a>tipo de enumeração remediable

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de status de execução do script de gerenciamento de dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Resultado desconhecido.|
|ignorados|1 |A execução do script de correção foi ignorada|
|sucesso|2 |O script de correção foi executado com êxito e corrigiu o estado do dispositivo|
|remediationFailed|3 |O script de correção foi executado com êxito, mas falhou ao corrigir o estado do dispositivo|
|scriptError|4 |Execução de script de correção encontrada e erro ou tempo limite esgotado|



