---
title: Tipo de numeração remediationState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7a47a880dbf067c455ca108fd8f80636810a6d31bc196b3c3198a87b089f6959
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164206"
---
# <a name="remediationstate-enum-type"></a>Tipo de numeração remediationState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de status de execução do script de gerenciamento de dispositivos.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Resultado desconhecido.|
|ignorado|1 |A execução do script de correção foi ignorada|
|sucesso|2|Script de correção executado com êxito e correção do estado do dispositivo|
|remediationFailed|3 |Script de correção executado com êxito, mas falhou ao remediar o estado do dispositivo|
|scriptError|4 |Execução de script de correção encontrada e erro ou tempo de execução|




