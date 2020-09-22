---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3d93ed616a73c69467a1a77cb27e6fb27a7ea553
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024294"
---
# <a name="defenderthreataction-enum-type"></a>tipo de enumeração defenderThreatAction

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação padrão do defender a ser executada em ameaças de malware detectadas.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Aplicar ação com base na definição de atualização.|
|ordena|1 |Limpe a ameaça detectada.|
|quarentena|2 |Colocar em quarentena a ameaça detectada.|
|remover|3 |Remova a ameaça detectada.|
|permitiu|4 |Permitir a ameaça detectada.|
|UserDefined|5 |Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.|
|Larga|6 |Bloquear a ameaça detectada.|






