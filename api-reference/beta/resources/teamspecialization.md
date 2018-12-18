---
title: tipo de enum teamSpecialization
description: Descreve o caso de uso especial para uma equipe.
author: nkramer
ms.openlocfilehash: 2e17f03374457ff8ddd9d3941eb56bebbec2dde6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348010"
---
# <a name="teamspecialization-enum-type"></a>tipo de enum teamSpecialization

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Indica se a [equipe](../resources/team.md) destina-se de um caso de uso específico. Especialização cada [equipe](../resources/team.md) tem acesso aos comportamentos exclusivos e experiências destinadas ao seu caso de uso. O padrão é 'Nenhum'.

## <a name="members"></a>Membros

| Membro             | Valor | Descrição                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| none               | 0     | Tipo de uma equipe que dá a experiência de equipe padrão padrão.          |
| unknownFutureValue | 7     | Sentinel valor reservado como um espaço reservado para expansão futura do enum. |
