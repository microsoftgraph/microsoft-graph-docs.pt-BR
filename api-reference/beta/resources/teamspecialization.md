---
title: tipo de enumeração Teamsspecialization
description: Descreve o caso de uso especial de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8700896c32a83a3e157186f405c435589ce03815
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345674"
---
# <a name="teamspecialization-enum-type"></a>tipo de enumeração Teamsspecialization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica se a [equipe](../resources/team.md) destina-se a um caso de uso específico. Cada especialização de [equipe](../resources/team.md) tem acesso a comportamentos e experiências exclusivos direcionados ao seu caso de uso. O padrão é ' nenhum '.

## <a name="members"></a>Membros

| Membro             | Valor | Descrição                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| Nenhuma               | ,0     | O tipo padrão para uma equipe que oferece a experiência de equipe padrão.          |
| educationStandard  | 1      | Equipe criada por um usuário educacional. Todas as equipes criadas pelo usuário educacional são do tipo edu. |
| educationClass     | 2      | Experiência de equipe otimizada para uma aula. Isso habilita a segmentação de recursos no O365. |
| educationProfessionalLearningCommunity | 3  | Experiência de equipe otimizada para um PLC. Saiba mais sobre o PLC [aqui](https://en.wikipedia.org/wiki/Professional_learning_community). |
| educationStaff     | 4      |  Tipo de equipe para uma experiência otimizada para a equipe em uma organização, onde o líder da equipe, como o principal, é o administrador e os professores são membros de uma equipe que vem com um bloco de anotações especializado. Para obter mais detalhes, consulte [bloco de anotações de equipe do OneNote para educação](https://www.onenote.com/staffnotebookedu). |
| unknownFutureValue | 7      | O valor de sentinela reservado como um espaço reservado para expansão futura da enumeração. |
