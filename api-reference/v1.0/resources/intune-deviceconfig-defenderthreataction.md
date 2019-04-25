---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d3d48415e55ad246f75ca9b32bd169ee102fc67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534315"
---
# <a name="defenderthreataction-enum-type"></a>tipo de enumeração defenderThreatAction

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação padrão do defender a ser executada em ameaças de malware detectadas.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Aplicar ação com base na definição de atualização.|
|ordena|1 |Limpe a ameaça detectada.|
|quarentena|2 |Colocar em quarentena a ameaça detectada.|
|remover|3 |Remova a ameaça detectada.|
|permitiu|4 |Permitir a ameaça detectada.|
|userDefined|5 |Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.|
|Larga|6 |Bloquear a ameaça detectada.|



