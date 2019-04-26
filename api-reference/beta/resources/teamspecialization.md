---
title: tipo de enumeração Teamsspecialization
description: Descreve o caso de uso especial de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c89f3ef993e55e28f5558f99c3ef87ad5174bc65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553649"
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
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/resources/teamspecialization.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
