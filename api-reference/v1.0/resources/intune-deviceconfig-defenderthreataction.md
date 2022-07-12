---
title: Tipo de enumeração defenderThreatAction
description: A ação padrão do Defender a ser tomada em ameaças de malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 18e8fe9b691e69cf63652dae9d7e8647694f1db9
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734330"
---
# <a name="defenderthreataction-enum-type"></a>Tipo de enumeração defenderThreatAction

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A ação padrão do Defender a ser tomada em ameaças de malware detectadas.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Aplicar ação com base na definição de atualização.|
|Limpo|1|Limpe a ameaça detectada.|
|quarentena|2|Colocar em quarentena a ameaça detectada.|
|Remover|3|Remova a ameaça detectada.|
|Permitir|4|Permitir a ameaça detectada.|
|Userdefined|5|Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.|
|Bloco|6 |Bloqueie a ameaça detectada.|





