---
title: tipo de enum teamSpecialization
description: Descreve o caso de uso especial para uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a2272ee085d0c265adc9ce2e3f1c598e45be21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930282"
---
# <a name="teamspecialization-enum-type"></a>tipo de enum teamSpecialization

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Indica se a [equipe](../resources/team.md) destina-se de um caso de uso específico. Especialização cada [equipe](../resources/team.md) tem acesso aos comportamentos exclusivos e experiências destinadas ao seu caso de uso. O padrão é 'Nenhum'.

## <a name="members"></a>Membros

| Membro             | Valor | Descrição                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| nenhum               | 0     | Tipo de uma equipe que dá a experiência de equipe padrão padrão.          |
| unknownFutureValue | 7     | Sentinel valor reservado como um espaço reservado para expansão futura do enum. |
